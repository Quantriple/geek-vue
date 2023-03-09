
<template>
<h1 @click="add" >{{count}}</h1>
  <form a></form>
</template>

<script setup>

import {ref} from "vue";

let count=ref(0);
function add() {
  count.value--;
}
  
</script>

<style scoped>

</style>