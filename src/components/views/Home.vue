<template>
<div class="container py-4">
    <div class="row">
       <pesquisar-vaga />
    </div>

    <div class="row mt-5">
        <div class="col-4">
            <div class="h-100 p-5 border bg-dark text-white">
                <p>Vagas Abertas</p>
                <h2>25</h2>
            </div>
        </div>

        <div class="col-4">
            <div class="h-100 p-5 border bg-primary text-white">
                <p>Proffsionais cadastrados</p>
                <h2>125</h2>
            </div>
        </div>

        <div class="col-4">
            <div class="h-100 p-5 border bg-success text-white">
                <p>Visitantes online</p>
                <h2>200</h2>
            </div>
        </div>

    </div>
</div>
</template>

<script>

import PesquisarVaga from '@/components/comuns/PesquisarVaga.vue'

export default {
    name: "Home",
    components: {
      PesquisarVaga
    },
    
    created() {
        console.log("Criado", this.teste);
    },
    activated() {
        console.log("Componente é ativado");
    },
    deactivated() {
        console.log("Componente é desativado");
    },
    beforeUnmount() {
        console.log("Antes de demonstar/destruir");
    },
    unmounted() {
        console.log("Demonstado/destruído");
    },
};
</script>

<style scoped></style>
