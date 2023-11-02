<script setup>
import { ref } from 'vue';

const tutorials = ref(['Vue 3 教程', 'IDEA 使用教程', 'Docker 教程'])
</script>

<template>
   <table border="1" width="600px">
    <tr>
      <td>序号</td>
      <td>名称</td>
    </tr>
    <tr v-for="(v, i) in tutorials" :key="i">
      <td>{{ i + 1 }}</td>
      <td>{{ v }}</td>
    </tr>
  </table>
</template>

<style scoped>
   .bg-back {
      background-color: black;
   }
   .red  {
      color: red;
   }

</style>
