<script setup>
  import { reactive } from 'vue';
  import Cabecalho from './components/Cabecalho.vue'
  import Formulario from './components/Formulario.vue'
  import ListaDeTarefas from './components/ListaDeTarefas.vue'
  import Membros from './components/Membros.vue'
  import BotaoZap from './components/BotaoZap.vue';
</script>

<template>
    <Cabecalho/>
    <Formulario/>
    <ListaDeTarefas/>
    <Membros/>
    <BotaoZap/>
</template>


