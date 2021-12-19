<script setup>
import Icons from "../atom/Icons.vue";
import BtnNav from "../atom/BtnNav.vue";
</script>

<template>
    <div class="bg-transparent py-4 flex flex-row justify-between items-center">
        <h1 class="font-bold text-3xl text-violet-500">
            <a href="#">Dimpang</a>
        </h1>
        <div class="flex flex-row gap-2">
            <BtnNav>
                <Icons class="h-8 w-8" name="message" />Social
            </BtnNav>
            <BtnNav>
                <Icons class="h-8 w-8" name="code" />Projects
            </BtnNav>
        </div>
    </div>
</template>



<style>
</style>