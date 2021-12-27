<script setup>
defineProps({
  title: String,
  description: String,
  image: String,
});
</script>

<template>
  <div class="flex flex-col gap-4">
    <div v-if="image">
      <img :src="image" class="rounded-xl" />
    </div>
    <div v-else class="bg-slate-200 h-52 w-full"></div>
    <h4 class="text-xl font-bold text-slate-900">{{ title }}</h4>
    <p class="text-base">{{ description }}</p>
  </div>
</template>
