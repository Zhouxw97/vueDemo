<script setup>
import { reactive, ref } from 'vue';

const obj = reactive({
  text: '<h1>🫅</h1>'
});

const path = ref("https://www.quanxiaoha.com")

const isActive = ref(true)

const classes = {
  red: 'red',
  background : 'bg-back'
}

</script>

<template>
 <div>
   <p><a v-bind:class="[classes.red,classes.background]">哈哈</a></p>
   <p><a v-bind:class="isActive ? 'red':'' ">哈哈</a></p>
 </div>
</template>

<style scoped>
   .bg-back {
      background-color: black;
   }
   .red  {
      color: red;
   }

</style>
