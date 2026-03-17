<script setup>
import { ref } from 'vue'

  
const count = ref(0)

function increment()
  {
    count.value++
  }
</script>

<template>
  <!-- 使此按钮生效 -->
  <!-- 1.监听按钮点击点击；2.调用一个加一的方法；3.把第二步的结果展示到按钮上-->
  <button @click = "increment">Count is: {{ count }}</button>
</template>