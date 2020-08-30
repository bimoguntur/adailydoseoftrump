<template>
  <b-jumbotron>
    <h1 class="display-4 font-weight-bold">A Daily Dose of Donald Trump 💕</h1>

    <p class="text-dark mt-5">
      “I think I am actually humble. I think I’m much more humble than you would understand.”
    </p>
    <p class="text-muted">
      -Donald Trump
    </p>

    <hr class="my-4">
    
    <b-button variant="primary" to="/quotes"> 
      MAKE AMERICA GREAT AGAIN
    </b-button>
  </b-jumbotron>

</template>

<script>
export default {
    head () {
        return {
          title: "Welcome to a daily dose of donald trump",
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

