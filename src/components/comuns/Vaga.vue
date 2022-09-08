<template>
    <div class="card">
        <div class="card-header bg-dark text-white">{{ tituloVagaTeste }}</div>
        <div class="card-body">
        <p>{{ descricaoVaga }}</p>
        </div>
        <div class="card-footer">
        <small class="text-muted">Salário: R$ {{ salario }} | Modalidade: {{ modalidade }} | Tipo: {{ tipo }} | Publicação: {{ publicacao }}</small>
        </div>
    </div>
</template>

<script>
export default {
    name: 'Vaga',
    // props: ['tituloVagaTeste', 'descricaoVaga', 'salario', 'modalidade', 'tipo', 'publicacao'],
    props: {
        // tipagem de dados vue
        tituloVagaTeste: String,
        descricaoVaga: String,
        salario:[Number, String],
        modalidade: String,
        tipo: String,
        publicacao: String
    },
    created() {  
         console.log(typeof this.tituloVagaTeste);      
        console.log(typeof this.descricaoVaga);
        console.log(typeof this.salario);
        console.log(typeof this.modalidade);
        console.log(typeof this.tipo);
        console.log(typeof this.publicacao);
    }
}
</script>