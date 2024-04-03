<script setup>
import { ref } from 'vue'

const count = ref(0)

const increment = () => {
  count.value++
}

function updateCount(event) {
  count.value = Number(event.target.value)
}
</script>

<template>
  <h1>{{ count }}</h1>
  <button @click="increment">+</button>
  <input @input="updateCount" />
</template>
