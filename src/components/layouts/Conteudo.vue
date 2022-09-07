<template>
  <div>
    <h1>{{ titulo }}</h1>
    <button @click="atualizarComponent()">Atualizar</button>
    <home></home>
    <publicar-vaga></publicar-vaga>
  </div>
</template>

<script>
import Home from "@/components/views/Home.vue";
import PublicarVaga from "@/components/views/PublicarVaga.vue";
export default {
  name: "Conteudo",
  components: {
    Home,
    PublicarVaga,
  },

  data: () => ({
    teste: "O componente foi criado",
    titulo: "Componente Conteudo",
  }),

  methods: {
    atualizarComponent() {
      this.titulo += "*";
    },
  },

  beforeCreate() {
    // não posso acessar estar propriedade antes do app ser criado
    console.log("Antes de criar", this.teste);
  },

  created() {
    // agora que o app foi criado, posso acessar o data
    console.log("Criado", this.teste);
  },

  beforeMount() {
    // posso recuperar dados por uma api e atribuir ao componente
    // para montar o app de fato
    console.log("Antes de Montar o template");
  },
  mounted() {
    console.log("Montado");
  },

  beforeUpdate() {
    // realcionado as atuliazações do code do componente
    console.log("Montado");
  },

  updated() {
    // realcionado as atuliazações do code do componente
    console.log("Atualizado");
  },

  beforeUnmount() {
    console.log("Antes de destruir");
  },

  unmounted() {
    console.log("destruido");
  },
  /*
  errorCaptured() {
    console.log("Erro capturado");
  },

  renderTracked() {
    console.log("Re-renderização rastreada");
  },

  renderTriggered() {
    console.log("Re-renderização acionada");
  },

  activated() {
    console.log("Componente Aativado");
  },

  deactivated() {
    console.log("Componente desativado");
  },
  */
};
</script>

<style module>
.teste {
  background-color: red;
}
#teste-2 {
  background-color: yellow;
}
</style>
