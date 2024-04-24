<script setup>
import Card from './Card.vue'
</script>

<template>
  <div class="grid grid-cols-4 gap-5">
    <Card
      img="/sneakers/sneakers-1.jpg"
      title="Мужские кроссовки Nike Blazer Mid Suede"
      :price="12999"
      :is-added="false"
      :is-favorite="true"
      :on-click-add="() => alert(111)"
    />
  </div>
</template>
