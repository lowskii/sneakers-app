<!-- eslint-disable vue/multi-word-component-names -->
<script setup>
defineProps({
  title: String,
  price: Number,
  img: String,
  isFavorite: Boolean,
  isAdded: Boolean,
  onClickAdd: Function,
  onClickfavorite: Function
})
</script>

<template>
  <div
    class="relative bg-white border border-slate-100 rounded-3xl p-8 cursor-pointer transition duration-300 hover:-translate-y-2 hover:shadow-xl"
  >
    <img
      @click="onClickfavorite"
      :src="isFavorite ? '/like-2.svg' : '/like-1.svg'"
      class="absolute top-8 left-8"
      alt="like 2"
    />
    <img :src="img" alt="Sneaker" />
    <p class="mt-2">{{ title }}</p>
    <div class="flex justify-between mt-5">
      <div class="flex flex-col">
        <span class="text-slate-400">Цена:</span>
        <b>{{ price }} руб.</b>
      </div>
      <img @click="onClickAdd" :src="isAdded ? '/checked.svg' : '/plus.svg'" alt="plus" />
    </div>
  </div>
</template>
