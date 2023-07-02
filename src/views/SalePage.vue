<template>
  <div class="form-group formSale">
    <div>
      <div class="divSpace">
      <label for="productName">Selecione o produto</label>
      <div class="divAlignmentItens">
        <select class="form-control productNameSelect" id="productName">
          <option value="" disabled selected>Selecione uma opção</option>
          <option value="opcao1">Pod</option>
        </select>
      </div>
      </div>
    </div>
  </div>
  <div class="form-group formSale">
    <div class="divSpace">
      <label for="brandProduct">Selecione a marca</label>
      <div class="divAlignmentItens">
        <select class="form-control productNameSelect" id="brandProduct">
          <option value="" disabled selected>Selecione uma opção</option>
          <option value="opcao1">Elfbar</option>
        </select>
      </div>
    </div>
  </div>
  <div class="form-group formSale">
    <div class="divSpace">
      <label>Valor do produto</label>
      <div class="divAlignmentItens">
        <input class="form-control productValue" type="text" placeholder="Digite aqui...">
      </div>
    </div>
  </div>
  <div class="form-group formSale">
    <div class="divSpace">
      <label>Nome do comprador</label>
      <div class="divAlignmentItens">
        <input class="form-control ownerName" size="32vh" type="text" placeholder="Digite aqui...">
      </div>
    </div>
  </div>
  <div class="form-group formSale">
    <div class="divSpace">
      <button class="btn btn-outline-dark">Inserir Venda</button>
    </div>
  </div>
</template>

<style scoped>


body{
  margin-top:15% !important;
}

.productNameSelect,
.productValue,
.ownerName {
  width: 32vh;
}


.formSale {
  display: flex;
  justify-content: center;
  align-items: center;
}

label {
  margin-right: 5px;
}

.divSpace {
  padding-top: 10px;
}

@media(max-width:400px) {
  .formSale {
    display: inherit;
  }

  .divAlignmentItens {
    display: flex;
    justify-content: center;
    align-items: center;
  }
}
</style>
