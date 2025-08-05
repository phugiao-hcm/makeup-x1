<template>
    <header class="bg-white shadow-md sticky top-0 z-50">
        <div
            class="max-w-7xl mx-auto flex items-center justify-between px-4 py-3"
        >
            <!-- Logo -->
            <NuxtLink to="/" class="flex items-center space-x-2">
                <span class="text-purple-700 font-bold text-xl md:text-2xl">
                    Makeup Phú Giáo
                </span>
            </NuxtLink>

            <!-- Desktop menu -->
            <nav
                class="hidden md:flex space-x-6 text-sm font-medium text-purple-700"
            >
                <NuxtLink to="/" class="hover:text-purple-500"
                    >Trang chủ</NuxtLink
                >
                <NuxtLink to="/" class="hover:text-purple-500"
                    >Dịch vụ</NuxtLink
                >
                <NuxtLink to="/" class="hover:text-purple-500"
                    >Mẫu Makeup</NuxtLink
                >
                <NuxtLink to="/" class="hover:text-purple-500"
                    >Liên hệ</NuxtLink
                >
            </nav>

            <!-- Mobile toggle -->
            <button class="md:hidden text-purple-700" @click="toggle = !toggle">
                <i class="fas fa-bars text-xl"></i>
            </button>
        </div>

        <!-- Mobile menu -->
        <div
            v-if="toggle"
            class="md:hidden bg-white border-t border-purple-200 px-4 py-2 space-y-2 text-sm text-purple-700"
        >
            <NuxtLink to="/" class="block hover:text-purple-500"
                >Trang chủ</NuxtLink
            >
            <NuxtLink to="/" class="block hover:text-purple-500"
                >Dịch vụ</NuxtLink
            >
            <NuxtLink to="/" class="block hover:text-purple-500"
                >Mẫu Makeup</NuxtLink
            >
            <NuxtLink to="/" class="block hover:text-purple-500"
                >Liên hệ</NuxtLink
            >
        </div>
    </header>
</template>

<script setup>
import { ref } from "vue";
const toggle = ref(false);
</script>

<style scoped>
@import url("https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css");
</style>
