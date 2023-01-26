<script setup>
import LikeSad from "./components/LikeSad.vue";
//import { ref } from 'vue';

//const stuID = ref("");
</script>

<template>
  <div v-for="n in 10" :key="n">
    <LikeSad></LikeSad>
    
  </div>


</template>

<style scoped>
h1 {
  color: aqua;
}
h2 {
  color: aquamarine;
}

</style>
