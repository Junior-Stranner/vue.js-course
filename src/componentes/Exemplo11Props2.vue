<!--Script-->
<script setup>

  //Obter Props
  const props = defineProps(['nome','idade','cidade','vetor','funcao']);

</script>


<!--HTML-->
<template>
    
    <p>Nome: {{nome}}</p>
    <p>Idade: {{idade}}</p>
    <p>Cidade: {{cidade}}</p>

    <ul>
      <li v-for="v of vetor">{{ v }}</li>
    </ul>

   <button @click="funcao">Clique Aqui</button>
</template>

      <!--Props Estáticos-->
<!--é um exemplo específico de atribuição de valores estáticos a props,
   e normalmente as props são usadas para passar dados dinâmicos de um componente pai 
   para um componente filho.-->

   <!--Props Dinâmicos-->
<!-- "props dinâmicos" referem-se à capacidade de passar dados de um componente pai para um componente filho de maneira dinâmica, 
  permitindo que o componente pai atualize as informações enviadas ao componente filho em tempo real.
   Isso é alcançado utilizando a diretiva v-bind (ou simplesmente :) para associar valores às props.-->