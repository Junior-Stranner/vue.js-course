<!--Script-->
<script setup>

let exibir = true;
let media = 8;

</script>

<!--HTML-->
<template>

  <h1 v-if="exibir">Hello world</h1>

<p v-if="media >= 7">Aprovado/a</p>
<p v-else-if="media >= 5">Em exame</p>
<p v-else>Reprovado/a</p>
</template>
