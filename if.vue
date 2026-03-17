<script setup>
import { ref } from 'vue'

const awesome = ref(true)

function toggle() {
  // ...
  awesome.value = !awesome.value
}
</script>

<template>
  <button @click="toggle">点击按钮代表爱yyl一天</button>
  <h1 v-if = "awesome">天数 + 1</h1>
  <h1 v-else>永远爱她</h1>
</template>