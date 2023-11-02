<script setup>
import { ref } from 'vue';
/* 节点中间用于放置 javascript 代码； */
const title = ref('插值表达式')
</script>

<template>
 <!--  节点中间用于放置 html 代码； -->
 <h1>{{title}}</h1>
</template>

<style scoped>
   /* 节点中间用于放置 css 代码； */
</style>
