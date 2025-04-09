<script setup lang="ts">
import { ref } from 'vue'

const welcome = ref('Hello Vue World!')
const description = ref('Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed dui eros, accumsan suscipit dapibus sed, convallis in ex. Mauris semper velit quis faucibus elementum.')

setTimeout(() => {
  welcome.value = 'Gracias!'
}, 2000)
</script>

<template>
  <div class="welcome">
    <div class="welcome__title">{{ welcome }}</div>
    <div class="welcome__description">{{ description }}</div>
  </div>
</template>

<style scoped lang="scss">
.welcome {
  margin-left: auto;
  margin-right: auto;
  width: 500px;
  background-color: yellow;
  text-align: center;
  padding: 20px;

  &__title {
    margin-bottom: 20px;
    font-size: 30px;
    font-weight: bold;
    color: red;
  }

  &__description {
    font-size: 24px;
    color: var(--vt-c-black-mute);
  }
}
</style>
