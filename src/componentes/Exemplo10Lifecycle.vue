<!--
  Lifecycle: São ações que podem acontecer em três estapas de um componente:

  - Antes da criação
  - Durante a criação
  - após a criação

-->

<!--Script-->
<script setup>
//Importar o REF
import { onMounted, ref } from 'vue';

  //variável
  let texto = ref('Hello World');

  //Lifecycle onMounted
  onMounted(() => {
  setTimeout(() => {
    texto.value = 'Alterando texto!';
  }, 3000);
});
</script>


<!--HTML-->
<template>
  
  <input type="text" v-model="texto">
  <p>{{texto}}</p>

</template>

<!-- quando o componente é montado, a função de onMounted é acionada após 3 segundos (devido ao setTimeout), 
  alterando o valor da variável texto para 'Alterando texto!'. Essa alteração será refletida automaticamente no campo de entrada
   de texto e no parágrafo, graças à reatividade do Vue.js.-->
