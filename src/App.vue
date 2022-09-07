<template>
  <div>
    <h1>componente APP</h1>
    <button @click="desmontarComponent()">
      Desmontar o Componente Conteudo
    </button>
    <topo-padrao />

    <conteudo v-if="visibilidate" />
  </div>
</template>

<script>
// o @ aponta pro src, para a raiz
import Conteudo from "@/components/layouts/Conteudo.vue";
import TopoPadrao from "@/components/layouts/TopoPadrao.vue";

// só posso usar os components depois de importar e registrar eles dentro
// do objeto literal components
export default {
  name: "App",
  data: () => ({
    visibilidate: true,
  }),

  methods: {
    desmontarComponent() {
      this.visibilidate = false;
    },
  },

  components: {
    Conteudo,
    TopoPadrao,
  },
};
</script>

<style scoped>
/* a tag scope mantem o estilo de cada compoente dentro de si mesmo */
/* em afetar os inferiores e superiores */
/* sem o scop , o ultimo estilo carregado é aplicado */
h1 {
  color: red;
}
</style>
