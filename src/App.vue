<template>
  <!-- <form-fitness /> -->
  <fetch-data />
</template>

<script>
import FetchData from "./components/FetchData.vue";
// import FormFitness from "./components/FormFitness.vue";

export default {
  name: "App",
  components: {
    FetchData,
    // FormFitness,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
