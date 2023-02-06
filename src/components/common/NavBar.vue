<script setup>
// modules
// components
import NavLink from './NavLink.vue'
// assets
import LeafIcon from '@/assets/svg/LeafIcon.vue'
//
const navItems = [
    {
        label: "Home",
        path: "/"
    },
    {
        label: "About",
        path: "/about"
    },
    {
        label: "Contact",
        path: "/contact"
    },
]
</script>
<template>
    <nav class="relative px-8 py-8 flex justify-between bg-primary-600">
        <RouterLink to="/">
            <LeafIcon />
        </RouterLink>
        <ul class="flex px-5">
            <NavLink v-for="item in navItems" :label="item.label" :path="item.path" />
        </ul>
    </nav>
</template>