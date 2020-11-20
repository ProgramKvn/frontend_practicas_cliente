<template>
  <div id="app">
    <!--Importando el componente de la navbar-->
    <Navbar />
    <router-view />
  </div>
</template>

<script>
import Navbar from "@/components/Componentes_Globales/Navbar.vue";

export default {
  name: "App",
  components: {
    Navbar,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}
</style>
