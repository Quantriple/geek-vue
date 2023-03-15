
<template>
<h1 @click="add" >{{count}}</h1>
  <form a></form>
</template>

<script setup>

import {ref} from "vue";

let count=ref(0);
let color =ref("blue");
function add() {
  count.value--;
  color.value =Math.random()>0.5?"blue":"red";
}
  
</script>

<style scoped>
h1 {
  color: v-bind(color)
}
</style>