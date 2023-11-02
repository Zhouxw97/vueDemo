<script setup>
import { reactive } from 'vue';
const obj = reactive({
  title: 'Hello World',
  num:1,
  num2:2,
  isSucces:true,
  arr:[1,2,3,4,5],
  subObj:{
    name:'subObj',
    age:18
  }
});

</script>

<template>
 <div>{{ obj.title }}</div>
 <div>{{ obj.num }}</div>
 <div>{{ obj.num > obj.num2 }}</div>

 <div>{{ obj.isSucces }}</div>

 <div>{{ obj.arr }}</div>

 <div>{{ obj.subObj }}</div>
 <div>{{ obj.subObj.name }}</div>

 <div>{{ obj.isSucces? 1:2 }}</div>
 <div v-text="obj.title"></div>

 <div v-once>{{ obj.title }}</div>
 <input v-model="obj.title" type="text">


</template>

<style scoped>
   
</style>
