<template>
  <div class="bg-white py-24">
    <div class="flex flex-col items-center">
      <h1 class="text-3xl text-gray-600">這是 posts/[postId] 的頁面</h1>
      <p class="my-8 text-3xl text-gray-600">
        匹配到的 Post Id:
        <span class="text-5xl font-semibold text-rose-500">{{ postId }}</span>
      </p>
    </div>
  </div>
</template>

<script setup>
const { postId } = useRoute().params;
</script>

<style lang="scss" scoped></style>
