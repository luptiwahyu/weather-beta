<script setup lang="ts">
import { ref } from 'vue'

const title = ref('Hello Vue!')

setTimeout(() => {
  title.value = 'Gracias!!'
}, 2000)
</script>

<template>
  <div>
    <div>
      <h1>{{ title }}</h1>
      <p>
        Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolorem temporibus eligendi dicta sit inventore quam
        nostrum tempore repellat quas a repellendus maxime amet dignissimos explicabo blanditiis, maiores dolore rem
        consequatur.
      </p>
    </div>

    <div class="welcome">
      <div class="welcome__title">Welcome</div>
      <div class="welcome__description">
        Lorem ipsum dolor sit amet, consectetur adipisicing elit. Totam deserunt saepe, rem ad eum, molestiae quae deleniti quam. Eius voluptas incidunt autem assumenda repudiandae sapiente dolorum ipsa nemo distinctio asperiores!
      </div>
    </div>
  </div>
</template>

<style scoped>
@reference '@/assets/styles/main.css';

p {
  @apply text-xl text-green-600;
}

.welcome {
  width: 500px;
  background-color: yellow;
  margin-top: 100px;
  margin-left: auto;
  margin-right: auto;
  padding: 30px;
}

.welcome__title {
  font-size: 20px;
  font-weight: bold;
  margin-bottom: 10px;
  color: blue;
}

.welcome__description {
  color: gray;
  font-style: italic;
}
</style>
