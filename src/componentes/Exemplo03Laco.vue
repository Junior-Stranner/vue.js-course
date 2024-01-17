<!--Script-->
<script setup>

  //vetor
  let nomes = ["Alice","Bruna","Caio","Daniel","Ellen"]

</script>

<!--HTML-->
<template>

   <ul>
    <li v-for="nome in nomes">{{nomes}}</li>
   </ul>
</template>
