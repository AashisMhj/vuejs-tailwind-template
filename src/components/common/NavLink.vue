<script setup>
// module
import {RouterLink, useRoute} from 'vue-router';
import {computed} from 'vue';
// components
// css assets
//
const route = useRoute();
const props = defineProps({
    label: String,
    path: String,
});
const is_active = computed(()=> props.path === route.path);
</script>

<template>
    <li :class="`text-white px-3 hover:text-gray-300 ${is_active ? 'text-green-900' : ''}`">
        <RouterLink :to="path">{{ label }}</RouterLink>
    </li>
</template>