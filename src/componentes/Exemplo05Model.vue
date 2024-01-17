<!--Script-->
<script setup>
//Importar o REF
import { ref } from 'vue';

  //variável
  let texto = ref('');
</script>


<!--HTML-->
<template>
  
  <input type="text" v-model="texto">
  <p>{{texto}}</p>

</template>

<!-- cria um campo de entrada de texto que permite ao usuário digitar um texto. O valor digitado é armazenado na variável
   reativa texto, e o mesmo é exibido em um parágrafo abaixo do campo de entrada de texto. O uso de ref torna a variável 
   texto reativa, o que significa que quaisquer alterações nela automaticamente 
  atualizarão a exibição no DOM.-->
