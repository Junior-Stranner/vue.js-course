<!--Script-->
<script setup>

  //Função de mensagem
  function mensagem(){
    alert('Executando a fução !');
  }
</script>


<!--HTML-->
<template>
 
 <input type="text" @keyup.enter="mensagem">
</template>

<!--Em resumo, este código cria uma aplicação Vue.js
   simples com um campo de entrada de texto, e quando você pressiona Enter nesse campo, a
    função mensagem é chamada, exibindo um alerta no navegador com a mensagem "Executando a função!".-->
