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
/* * {
  background-color: #f7f7f7;
} */

</style>
