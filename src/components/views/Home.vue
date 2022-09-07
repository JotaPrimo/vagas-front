<template>
  <div class="container py-4">
    <div class="row">
      <div class="h-100 p-5 bg-light border rounded-3">
        <h2>Pesuisar Vagas</h2>
        <div class="row">
          <div class="col">
            <div class="form-group">
              <label for="">Titulo do Vaga</label>
              <input type="text" class="form-control" placeholder="Pesquisar" />
              <small class="form-text text-muted"
                >Informe palavras relacionadas com o titulo da vaga</small
              >
            </div>
          </div>
        </div>

        <div class="row">
          <div class="col">
            <button class="btn btn-primary btn-sm">Buscar</button>
          </div>
        </div>
      </div>
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
export default {
  name: "Home",
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
