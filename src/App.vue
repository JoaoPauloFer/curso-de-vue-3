<template>
  <main class="columns is-gapless is-multiline">
    <div class="column is-one-quarter">
      <BarraLateral />
    </div>
    <div class="column is-three-quarter">
      <FormularioTarefa />
      <div class="lista">
        <Tarefa />
        <Tarefa />
        <Tarefa />
      </div>
    </div>
  </main>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import BarraLateral from './components/BarraLateral.vue';
import FormularioTarefa from './components/FormularioTarefa.vue';
import Tarefa from './components/CompTarefa.vue';


export default defineComponent({
    name: "App",

    components: { 
      BarraLateral,
      FormularioTarefa,
      Tarefa
      }
});
</script>

<style>
.lista{ 
  padding: 1.5rem;
}
</style>
