<script setup>
defineProps({
    title: String,
    img: String
})
</script>
<template>
  
<div class="flex items-center border border-slate-200 p-4 rounded-xl gap-4">
    <img class="w-16 h-16" :src="img" alt="Sneaker" />

    <div class="flex flex-col justify-between">
        <p>{{ title }}</p>

        <div class="flex justify-between mt-2">
            <b>1205 руб.</b>
            <img class="opacity-40 hover:opacity-100 cursor-pointer transition" src="/close.svg" alt="close" />
        </div>
    </div>
</div>
</template>