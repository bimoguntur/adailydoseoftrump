<template>
    <b-container>
        <p class="h4 text-dark" >About</p>
        <hr />

        <p class="h6 text-secondary">
            Welcome to A Daily Dose of Trump.

            Here we give you the greatest quotes of our greatest man in history. <br>
            <br>
            America first. <br>
            <br>
            Make America Great Again.
        </p>

    </b-container>
</template>

<script>
export default {
    head () {
        return {
            title: 'About the App',
            meta: [
                { 
                    hid: "description",
                    name: "description",
                    content: "Best place for a daily dose of Trump's quotes"
                }   
            ]
        }
    }
}
</script>