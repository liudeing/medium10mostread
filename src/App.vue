<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <CreatePDF msg="medium阅读量最高的10篇文章翻译"/>
</template>

<script>
import CreatePDF from "@/components/CreatePDF.vue";

export default {
  name: 'App',
  components: {
    CreatePDF
  }
}
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
