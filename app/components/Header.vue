<template>
  <header class="w-full bg-white shadow-sm py-4 px-6">
    <div class="max-w-screen-xl mx-auto flex items-center justify-between">
      <!-- Logo -->
      <div class="flex items-center gap-2">
        <img src="/images/logo.png" alt="Logo" class="h-10" />
      </div>

      <!-- Desktop Navigation -->
      <nav
        class="hidden lg:flex items-center gap-8 text-sm font-medium text-gray-800"
      >
        <NuxtLink to="/" class="hover:text-orange-500"
          >COMPO PHÒNG NGỦ</NuxtLink
        >
        <NuxtLink to="/" class="hover:text-orange-500">BÀN ĂN</NuxtLink>
        <NuxtLink to="/" class="hover:text-orange-500">TỦ QUẦN ÁO</NuxtLink>
        <NuxtLink to="/" class="hover:text-orange-500">BÀN TRANG ĐIỂM</NuxtLink>
        <NuxtLink to="/" class="hover:text-orange-500">SẢN PHẨM KHÁC</NuxtLink>
      </nav>

      <!-- Call Button (always visible) -->
      <button
        class="w-10 h-10 rounded-full bg-orange-500 text-white flex items-center justify-center"
      >
        <svg
          xmlns="http://www.w3.org/2000/svg"
          class="h-5 w-5"
          fill="none"
          viewBox="0 0 24 24"
          stroke="currentColor"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            d="M3 5h2l3.5 7-1.5 2a17 17 0 006.5 6.5l2-1.5 7 3.5v2a1 1 0 01-1 1h-3a19 19 0 01-19-19V6a1 1 0 011-1z"
          />
        </svg>
      </button>

      <!-- Hamburger (Mobile only) -->
      <button
        @click="menuOpen = !menuOpen"
        class="lg:hidden ml-4 text-gray-800 focus:outline-none"
      >
        <svg
          class="w-6 h-6"
          fill="none"
          stroke="currentColor"
          stroke-width="2"
          viewBox="0 0 24 24"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M4 6h16M4 12h16M4 18h16"
          />
        </svg>
      </button>
    </div>

    <!-- Mobile Menu -->
    <div v-if="menuOpen" class="lg:hidden mt-4 px-6">
      <div class="flex flex-col space-y-3 text-sm font-medium text-gray-800">
        <NuxtLink to="/" class="hover:text-orange-500"
          >COMPO PHÒNG NGỦ</NuxtLink
        >
        <NuxtLink to="/" class="hover:text-orange-500">BÀN ĂN</NuxtLink>
        <NuxtLink to="/" class="hover:text-orange-500">TỦ QUẦN ÁO</NuxtLink>
        <NuxtLink to="/" class="hover:text-orange-500">BÀN TRANG ĐIỂM</NuxtLink>
        <NuxtLink to="/" class="hover:text-orange-500">SẢN PHẨM KHÁC</NuxtLink>
      </div>
    </div>
  </header>
</template>

<script setup>
import { ref } from "vue";
const menuOpen = ref(false);
</script>
