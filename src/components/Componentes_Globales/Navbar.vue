<template>
  <!--El siguiente componente permite al usuario navegar a través de los demás componentes del sitio web; La navbar se mantiene presente en cada página del sitio-->
  <div id="Navbar">
    <b-navbar type="dark" variant="dark" fixed="top">
      <b-navbar-brand>El Pajarito SV</b-navbar-brand>
      <b-navbar-nav class="ml-auto">
        <!--Aquí comienza el primer elemento de la navbar-->
        <b-nav-item right>
          <router-link :to="{ path: '/' }">Inicio</router-link>
        </b-nav-item>
        <!--Gracias al elemento ROUTER LINK y al path que este ofrece, podemos agregar la funcionalidad de VIEWS para brindar una navegación dentro del sitio web (utilizando <router-link>), manteniendo el código ordenado y limpio-->

        <!--Aquí termina el primer elemento de la navbar-->

        <!--Aquí comienza el segundo elemento de la navbar-->
        <b-nav-item right>
          <router-link :to="{ path: '/blog' }">Blog</router-link>
        </b-nav-item>
        <!--Aquí termina el segundo elemento de la navbar-->

        <!--Aquí comienza el tercer elemento de la navbar-->
        <b-nav-item>
          <router-link :to="{ path: '/conocenos' }">Conócenos</router-link>
        </b-nav-item>
        <!--Aquí termina el tercer elemento de la navbar-->

        <!--Aquí comienza el cuarto elemento de la navbar-->
        <b-nav-item>
          <router-link :to="{ path: '/contacto' }">Contáctanos</router-link>
        </b-nav-item>
        <!--Aquí termina el cuarto elemento de la navbar-->
      </b-navbar-nav>
    </b-navbar>
  </div>
  <!--Aquí termina la navbar-->
</template>

<script>
export default {
  name: "Navbar",
};
</script>

<style scoped>
#Navbar {
  margin-bottom: 35px;
}
#Navbar a {
  font-weight: bold;
  color: #ffffff;
}
/*Cuando el usuario hace clic en el elemento, se mantiene activo y cambia de color*/
#Navbar a.router-link-exact-active {
  color: #42b983;
}
</style>