<template>
    <div
        :class="`group inline-flex h-10 w-10 overflow-hidden items-center cursor-pointer float-left transition ease-out duration-500 hover:w-40 hover:bg-white hover:shadow-xl ${shadowColor} rounded-full`"
    >
        <div :class="`p-1 ${bgColor} rounded-full`">
            <Icons :name="icon" :class="`w-8 h-8 ${textColor} group-hover:text-white`" />
        </div>
        <div :class="`hidden ${textColor} group-hover:block m-2`">{{ text }}</div>
    </div>
</template>

<script setup>
import Icons from '../atom/Icons.vue';

defineProps({
    icon: String,
    text: String,
    bgColor: String,
    shadowColor: String,
    textColor: String,
})

</script>