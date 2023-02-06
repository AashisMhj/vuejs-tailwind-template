<script setup>
defineProps({
    text: {type: String, required: true}
})
</script>
<template>
    <h1 class="h-1 text-white font-sans text-7xl">{{ text }}</h1>
</template>