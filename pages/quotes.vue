<template>
    <b-container>
      
        <h5 class="lg text-dark" >MAGA! This is your daily dose of Trump.</h5>
        <hr />
        
        <b-card bg-variant="light" class="mt-4">
            <b-card-title  class="h2 text-black">{{quote.value}}</b-card-title>
            <b-card-text class="h5 font-weight-light text-muted">
                Donald Trump
            </b-card-text>
            <b-card-text>
                <a :href="source" class="h6 font-weight-light">SEE SOURCE</a>
            </b-card-text> 

        </b-card>
        <div>
            <b-button @click="$fetch" block variant="outline-primary" class="mt-3">MORE, PLEASE</b-button>
        </div>
            
    </b-container>
</template>

<script>
import axios from 'axios';

export default {
    
    data() {
        return {
            quote: [],
            source: []
            
        };
    },

    async fetch() {
        const config = {
            header: {
                Accept: 'application/hal+json' 
            }
        };
        
        try {
            const res = await axios.get('https://api.tronalddump.io/random/quote', config);

            this.quote = res.data;
            this.id = res.data.quote_id;
            this.source = res.data._embedded.source[0].url;
            console.log(res)
        } catch (err) {
            console.log(err);
        }

    },
    methods: {
        refresh() {
            this.$fetch()
        }
    }

}
</script>