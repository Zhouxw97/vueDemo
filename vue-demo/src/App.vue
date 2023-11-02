<script setup>
import { reactive } from 'vue';

const obj = reactive({
  text: '<h1>🫅</h1>'
});

</script>

<template>
 <div v-text="obj.text"></div>
 <div v-html="obj.text"></div>
</template>

<style scoped>
   
</style>
