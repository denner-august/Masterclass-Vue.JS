<script setup>
import FirtComponent from "./components/Primeiro.vue";
import WithDate from "./components/withDate.vue";
import ComponentDadosPrimitivos from "./components/ComponentDadosPrimitivos.vue";
import ComponentDadosNaoPrimitivos from "./components/ComponentDadosNaoPrimitivos.vue";
import DataBinding from "./components/dataBinding.vue";
import WiithPros from "./components/withProps.vue";
import ListeningEvent from "./components/listeningEvent.vue";
import PropsComputadas from "./components/propsComputadas.vue";
</script>

<template>
  <header>Vue</header>
  <PropsComputadas />
  <ListeningEvent />
  <WiithPros item="teste" :preco="10" />
  <WiithPros item="caderno" v-bind:preco="50.3" />
  <DataBinding />
  <ComponentDadosNaoPrimitivos />
  <ComponentDadosPrimitivos />
  <FirtComponent />
  <WithDate />
</template>
