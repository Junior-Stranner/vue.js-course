<!--Script-->
<script setup>

    //Import
    import Exemplo11Props2 from './Exemplo11Props2.vue';

    //Variáveis
    let cidade = 'Balneário Camboriú';
    let cidades = ['São Paulo','Rio de Janeiro','Curitiba','Bahia','Fortaleza'];

    //Função
    function mensagem(){
      alert('Funcção criada no componente: Exemplo11Props1');
    }

</script>

<!--HTML-->
<template>
  
  <Exemplo11Props2 nome="Junior" idade="22" :cidade="cidade" :vetor="cidades" funcao="mensage"></Exemplo11Props2>

</template>

      <!--Props Estáticos-->
<!--é um exemplo específico de atribuição de valores estáticos a props,
   e normalmente as props são usadas para passar dados dinâmicos de um componente pai 
   para um componente filho.-->

   <!--Props Dinâmicos-->
<!-- "props dinâmicos" referem-se à capacidade de passar dados de um componente pai para um componente filho de maneira dinâmica, 
  permitindo que o componente pai atualize as informações enviadas ao componente filho em tempo real.
   Isso é alcançado utilizando a diretiva v-bind (ou simplesmente :) para associar valores às props.-->

