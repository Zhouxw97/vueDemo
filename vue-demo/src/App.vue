<script setup>
import { ref } from 'vue';
/* 节点中间用于放置 javascript 代码； */
const count = ref(0)
</script>

<template>
 <!--  节点中间用于放置 html 代码； -->
 <h1>Hello vue3!</h1>
 <button @click="count++">count: {{count}}</button>
</template>

<style scoped>
   /* 节点中间用于放置 css 代码； */
</style>
