<script setup>
import Icons from "../atom/Icons.vue";

defineProps({
    title: String,
    icon: String,
});
</script>

<template>
    <div
        class="bg-white h-36 w-36 rounded-2xl font-semibold flex flex-col items-center justify-center"
    >
        <Icons class="w-12 h-12 mb-4" :name="icon" />
        <p>{{ title }}</p>
    </div>
</template>

