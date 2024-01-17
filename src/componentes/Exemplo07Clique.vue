<!--Script-->
<script setup>

  //Função
  function mensagem(){
    alert('Trabalhando com eventos de clique!');
  }
</script>


<!--HTML-->
<template>
 
  <button @click="mensagem"> Clique aqui</button>
</template>


<!-- aplicação Vue.js simples que responde a eventos de clique em um botão, 
  demonstrando uma mensagem ao usuário quando o botão é pressionado.-->