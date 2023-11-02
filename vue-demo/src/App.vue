<script setup>
import { reactive, ref } from 'vue';

const obj = reactive({
  text: '<h1>🫅</h1>'
});

const path = ref("https://www.quanxiaoha.com")

</script>

<template>
 <div v-text="obj.text"></div>
 <div v-html="obj.text"></div>

 <a :href="path" style="display: block;">小哈教程</a>
 <a v-bind:href="path" style="display: block;">小哈教程</a>
</template>

<style scoped>
   
</style>
