<template>
  <div class="componente">
    <h1>Component com data binding</h1>
    {{ valor }}
    <!--
      <input
      type="text"
      :value="valor"
      @:input="(e) => (valor = e.target.value)"
      />
      -->
    <input type="text" v-model="valor" />
  </div>
</template>

<script setup>
import { ref } from "vue";
const valor = ref("vue é muito legal");
</script>

<style scoped>
div {
  display: flex;
  flex-direction: column;
  align-items: center;
}

input {
  width: 50vw;
  text-align: center;
  margin-top: 1rem;
}
</style>
