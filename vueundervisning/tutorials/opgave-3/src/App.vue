<script setup>
  import { ref } from 'vue';
  let fornavn = ref('');
  let efternavn = ref('');
  let email = ref('');
  let dato = ref('');
  

  function onSubmit (){

  }

</script>

<template>
  
<div>
  <input type="text" v-model="fornavn" />
  <input type="text" v-model="efternavn"/>
  <input type="text" v-model="email"/>
  <input type="text" v-model="dato"/>
</div>

<div>
  <h3>Navn = {{ fornavn + " " + efternavn }}</h3>
  <p>email = {{ email }}</p>
  <p>Fødselsdato = {{ dato }}</p>
  <button v-on:click="onSubmit">Gem information</button>
  <p>{{ info }}</p>
</div>



</template>

<style scoped>  

</style>
