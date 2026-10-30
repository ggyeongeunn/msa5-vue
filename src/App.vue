<script setup>
import { ref } from 'vue';

const count = ref(0);
</script>

<template>
  <div class="btn-cnt" @click="count++">Count is {{ count }}</div>
  <button @click="count = 0">Count Reset</button>
</template>

<style>
.btn-cnt { 
  width: fit-content;
  margin: 50px auto;
  padding: 10px 20px;
  border: 1px solid #cdd1d5;
  border-radius: 4px;
  cursor: pointer;
  transition: 0.3s;
}
.btn-cnt:hover{
  background-color: #f4f5f6;
}
button{
  width: 120px;
  padding: 10px 20px;
  margin: 0 auto;
  border: 1px solid #cdd1d5;
  border-radius: 4px;
  background-color: #fff;
  color: #454545;
  cursor: pointer;
  transition: 0.3s;
}
button:hover{
  background-color: #f4f5f6;
}
</style>