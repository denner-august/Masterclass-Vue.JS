<script setup>
import FirtComponent from "./components/Primeiro.vue";
import WithDate from "./components/withDate.vue";
import ComponentDadosPrimitivos from "./components/ComponentDadosPrimitivos.vue";
import ComponentDadosNaoPrimitivos from "./components/ComponentDadosNaoPrimitivos.vue";
import DataBinding from "./components/dataBinding.vue";
</script>

<template>
  <header>Vue</header>
  <DataBinding />
  <ComponentDadosNaoPrimitivos />
  <ComponentDadosPrimitivos />
  <FirtComponent />
  <WithDate />
</template>
