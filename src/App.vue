<template>
  <cabecalhoSite></cabecalhoSite>
  <corpoSite></corpoSite>
</template>

<script>
import cabecalhoSite from './components/pages/homepage/cabecalho.vue'
import corpoSite from './components/pages/homepage/corpo.vue'

export default {
  name: 'App',
  components: {
    cabecalhoSite,
    corpoSite,
  }
}
</script>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  font-family: "poppins";
}
html, body {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
  width: 100%;
  height: 100%;
}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}


</style>