<template>
	<button class="cursor-pointer bg-[#F54D0C] w-[150px] h-[50px] z-5 text-white font-bold rounded-xl p-4 text-center" @mouseover="toggleHover('Soon')"
        @mouseleave="toggleHover('Join IDO sale')">
            {{ MouseOver.value }}
    </button>
</template>
<script setup>
    import { reactive } from 'vue';
    const MouseOver = reactive({ value: 'Join IDO sale' });
    const toggleHover = (text) => {
        MouseOver.value = text;
    }
</script>