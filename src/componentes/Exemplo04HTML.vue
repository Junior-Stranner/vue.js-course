<!--Script-->
<script setup>
  //variável
  let texto = '<p style="color:red" Aprendendo a divertiva v-html</p>';
</script>

<!--HTML-->
<template>
  
  <!--Maior exemplo é se eu adicionar o style , só pegará no html e não no Interpolacao-->
  <div v-html="texto"></div>

  <!--faz o msm porem não tem foco html-->
  <div>{{texto}}</div>
</template>


<!--Um ponto importante a ser considerado ao usar v-html é garantir que o conteúdo inserido seja seguro para evitar
   ataques de injeção de código (XSS). Certifique-se de sanitizar e validar cuidadosamente qualquer conteúdo HTML
   dinâmico que você estiver incorporando.-->