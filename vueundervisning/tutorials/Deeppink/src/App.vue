<script setup>
import { ref } from 'vue';
const vandcykel = ref('');

function onSubmit (){
  alert (vandcykel.value);
}

</script>

<template>

  <input type="text" v-model="vandcykel" />
  <button v-on:click="onSubmit">
    KANP LOL
  </button>
  {{ vandcykel }}
  
</template>

