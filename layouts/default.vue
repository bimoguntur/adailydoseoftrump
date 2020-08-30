<template>
  <b-container>
    <div class="col-lg-8 mx-auto justify-content-center">
      <lauraHeader />
      <Nuxt class="mt-5"/>
      
    </div>
  </b-container>
</template>

<script>
import lauraHeader from "../components/appHeader";

export default {
  components: {
    lauraHeader,
  }
}
</script>

<style>

html {
  height: 100%;
}

body {
  min-height: 100vh;
}

footer {
  margin-top: auto;
  background-color: #121212;
}
</style>
