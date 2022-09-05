<template>
  <div>  
      <p>Conteudo do Conteudo</p>  
      <home></home>
      <publica-vaga />
  </div>
</template>

<script>

import Home from '../views/Home.vue' 
import PublicaVaga from '../views/PublicaVaga.vue'

export default {
    name: 'Conteudo',
    components: {
      Home,      
      PublicaVaga
    }
  }
</script>


<style></style>
