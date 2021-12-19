<template>
    <a
        :href="url"
        :class="`group inline-flex h-10 w-10 bg-transparent overflow-hidden items-center cursor-pointer float-left transition-all ease-out duration-300 hover:w-40 hover:bg-white hover:shadow-xl ${shadowColor} rounded-full`"
        target="_blank"
        rel="noopener noreferrer"
    >
        <div
            :class="`text-center p-1 ${bgColor} rounded-full transition-all ease-out duration-300`"
        >
            <Icons
                :name="icon"
                :class="`w-8 h-8 ${textColor} group-hover:text-white transition-all ease-out duration-300`"
            />
        </div>
        <span :class="`${textColor} m-2`">{{ text }}</span>
    </a>
</template>

<script setup>
import Icons from '../atom/Icons.vue';

defineProps({
    url: String,
    icon: String,
    text: String,
    bgColor: String,
    shadowColor: String,
    textColor: String,
})

</script>