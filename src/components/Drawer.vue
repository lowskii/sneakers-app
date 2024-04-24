<!-- eslint-disable vue/multi-word-component-names -->
<script setup>
import DrawerHead from './DrawerHead.vue'
import CartListItem from './CartListItem.vue';
</script>

<template>
  <div class="fixed top-0 left-0 h-full w-full bg-black opacity-50 z-10"></div>
  <div class="bg-white w-96 fixed right-0 top-0 h-full p-8 z-20">
    <DrawerHead />
    <CartListItem />

    <div class="flex flex-col gap-4 mt-7">
      
      <div class="flex gap-2">
        <span>Итого:</span>
        <div class="flex-1 border-b border-dashed"></div>
        <b>
          1205 руб.
        </b>
      </div>
    
      <div class="flex gap-2">
        <span>Налог 5%</span>
        <div class="flex-1 border-b border-dashed"></div>
        <b>
          50 руб.
        </b>
      </div>

      <button
      disabled = ""
      class="mt-4 bg-lime-500 w-full disabled:bg-slate-300 rounded-xl py-3 text-white hover:bg-lime-600 active:bg-lime-700 cursor-pointer">
        Оформить заказ
      </button>

    </div>
  </div>
</template>
 