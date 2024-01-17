<!--Script-->
<script setup>

  //variável
  let validacao = false;
</script>


<!--CSS-->
<style>
.ok{color:green;}

.falha{color:red}
</style>

<!--HTML-->
<template>

 <p v-bind:class="validacao ? 'ok' : 'falha'">Utilizando diretiva class</p>

</template>

<!-- este código Vue.js utiliza a diretiva v-bind:class para aplicar estilos condicionais ao parágrafo (<p>)
   com base no valor da variável validacao. Se validacao for true, a mensagem será exibida com estilo verde (.ok); 
   caso contrário, será exibida com estilo vermelho (.falha).
   Isso demonstra como a diretiva v-bind:class pode ser usada para aplicar estilos dinamicamente com base no estado do componente.-->
