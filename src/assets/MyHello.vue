<script setup>
defineProps({
  name: String,
  price: Number
})
</script>
<template>
  <div class="shoes">
    <h1>{{ name }}</h1>
    <h2>Цена: {{ price }}</h2>
  </div>
</template>

<style scoped>
.shoes {
  border: 1px solid blue;
  padding-left: 15px;
}
</style>
