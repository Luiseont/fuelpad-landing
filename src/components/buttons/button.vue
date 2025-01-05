<template>
	<button class="cursor-pointer bg-[#FA140A] w-[150px] h-[50px] text-white font-bold rounded-xl p-4 text-center text-sm lg:text-md" @mouseover="toggleHover('Soon')"
        @mouseleave="toggleHover('Enter App')">
            {{ MouseOver.value }}
    </button>
</template>
<script setup>
    import { reactive } from 'vue';
    const MouseOver = reactive({ value: 'Enter App' });
    const toggleHover = (text) => {
        MouseOver.value = text;
    }
</script>