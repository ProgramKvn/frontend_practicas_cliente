<template>
  <div id="Inicio">
    <!--En esta vista, se decidió crear aquí el sistema Grid para mostrar de forma estructurada 3 componentes-->
    <b-container fluid>
      <b-row>
        <b-col cols="9" class="p-2">
          <!--El primer y segundo componente dispondrán de 9 columnas de 12 en total-->
          <Slide />
          <Mostrar_Entrada />
        </b-col>
        <b-col cols="3" class="p-2">
          <!--El tercer componente dispondrán de 3 columnas de 12 en total-->
          <Sidebar />
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>
import Slide from "@/components/Inicio/Slide.vue";
import Mostrar_Entrada from "@/components/Inicio/Mostrar_Entrada.vue";
import Sidebar from "@/components/Componentes_Globales/Sidebar.vue";

export default {
  name: "Inicio",
  components: {
    Slide,
    Mostrar_Entrada,
    Sidebar,
  },
};
</script>

<style scoped>
</style>