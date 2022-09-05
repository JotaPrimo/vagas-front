<template>  
    <div>
      
      <topo-padrao />

      <conteudo />

    </div>
</template>

<script>
import Conteudo from './components/layouts/Conteudo.vue'
import TopoPadrao from './components/layouts/TopoPadrao.vue'

// só posso usar os components depois de importar e registrar eles dentro
// do objeto literal components
export default {
  name: 'App',
  components: {
    Conteudo,
    TopoPadrao
  }
}
</script>

<style>

</style>
