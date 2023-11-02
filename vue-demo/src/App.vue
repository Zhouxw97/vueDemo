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

const isShow = ref(true)

const type = ref(1)

</script>

<template>
 <div>
   <p><a v-bind:class="[classes.red,classes.background]">哈哈</a></p>
   <p><a v-bind:class="isActive ? 'red':'' ">哈哈</a></p>
 </div>
  <!-- 通过 v-if 指令判断 isShow 是否为 true, 若是则渲染 <a> 标签，否则不渲染 -->
   <a href="https://www.quanxiaoha.com" v-if="isShow">犬小哈教程</a>
   <a href="https://www.quanxiaoha.com" v-else-if="type === 2">犬小哈教程2</a>
    <a href="https://www.quanxiaoha.com" v-else-if="type === 3">犬小哈教程3</a>
   <div v-else>www.quanxiaoha.com</div>
</template>

<style scoped>
   .bg-back {
      background-color: black;
   }
   .red  {
      color: red;
   }

</style>
