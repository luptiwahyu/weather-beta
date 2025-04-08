<script setup lang="ts">
import { ref } from 'vue'

const welcome = ref('Hello Vue World!')

setTimeout(() => {
  welcome.value = 'Gracias!'
}, 2000)
</script>

<template>
  <h1>{{ welcome }}</h1>
</template>

<style scoped>
</style>
