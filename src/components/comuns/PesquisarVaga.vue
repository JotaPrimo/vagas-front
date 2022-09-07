<template>

<div class="h-100 p-5 bg-light border rounded-3">
    <h2>Pesuisar Vagas</h2>
    <div class="row">
        <div class="col">
            <div class="form-group">
                <label for="">Titulo do Vaga</label>
                <input type="text" class="form-control" placeholder="Pesquisar" />
                <small class="form-text text-muted">Informe palavras relacionadas com o titulo da vaga</small>
            </div>
        </div>
    </div>

    <div class="row">
        <div class="col">
            <button class="btn btn-primary btn-sm">Buscar</button>
        </div>
    </div>
</div>

</template>

<script>
export default {
    name: 'PesquisarVaga'
}
</script>
