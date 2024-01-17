<!--Script-->
<script setup>

  //Função para validar o formulário
  function validaFormulario(event){ //event palavra Reservada
    alert('Formulário enviado !');

    event.preventDefault();  //não irá liberar o redirecionamento sem que todos os campos de um cadastro for preenchido
  }
</script>


<!--HTML-->
<template>
     <form action="https://github.com/Junior-Stranner" @submit="validaFormulario">
      <input type="submit" value="Enviar Formulário">
    </form>
</template>

             <!-- 1 versão Aula 14 -->
<!--Quando o usuário preenche o formulário e o envia, a função validaFormulario é chamada, exibindo um alerta no navegador
   com a mensagem "Formulário enviado!".Este é um exemplo básico de como lidar com eventos de formulário em um componente Vue.js.-->

              <!-- 1 versão Aula 15 -->
<!-- Sobre  event.preventDefault(); Essa técnica é comumente usada para validar dados de formulário,
   interagir com APIs antes de enviar dados, ou para impedir envios acidentais 
  de formulários enquanto ainda está manipulando a entrada do usuário.-->
