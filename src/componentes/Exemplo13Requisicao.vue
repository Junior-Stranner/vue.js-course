<!--Script-->
<script setup>

    import {onMounted ,ref} from 'vue';

   //Vetor contendo as postagens
   let vetor = ref([]);


  // onMounted
  onMounted(() => {
        fetch('https://jsonplaceholder.typicode.com/posts')
        .then(retorno => retorno.json())
        .then(retorno => vetor.value = retorno);
    });
 
</script>
   

<!--HTML-->
<template>
    
    <h1>Requisições</h1>

    <table>
         <tr v-for="v in vetor">
            <td>{{ v.userId }}</td>
            <td>{{ v.id }}</td>
            <td>{{ v.title }}</td>
            <td>{{ v.body }}</td>
         </tr>
    </table>
 
</template>
