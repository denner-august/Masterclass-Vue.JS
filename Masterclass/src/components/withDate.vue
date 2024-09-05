<template>
  <div>
    <h1>Component with date</h1>
    <p>Name: {{ ProdutName }} - code {{ ProdutCode }}</p>
  </div>
</template>

<style scoped>
div {
  text-align: center;
  border: 2px solid rgb(10, 69, 4);
  background-color: #050d04;
  border-radius: 15px;
  margin: 30px;
  padding: 10px;
}
</style>

<script setup>
const ProdutName = "apontador";
const ProdutCode = "#500";
</script>

<!-- <script>

//option API
export default {
  data: function () {
    return {
      ProdutName: "Caderno",
      ProdutCode: "#321",
    };
  },
};



// composition API

export default {
    setup: function () {
        const ProdutName = "lapis";
        const ProdutCode = "#443";
        return { ProdutName, ProdutCode };
    },
};
</script>
-->
