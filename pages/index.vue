<script setup></script>

<template>
  <div class="bg-white py-24">
    <div class="flex flex-col items-center">
      <h1 class="text-6xl font-semibold text-gray-800">這裡是首頁</h1>

      <div class="my-4 flex gap-x-4">
        <nuxt-link to="/about">前往 About</nuxt-link>
        <nuxt-link to="/contact">前往 Contact</nuxt-link>
        <nuxt-link to="/posts">前往 posts</nuxt-link>
        <nuxt-link to="/docs">前往 docs</nuxt-link>
      </div>
    </div>
  </div>
</template>

<style lang="scss" scoped></style>
