<template>
  <div class="m-4 bg-white">
    <p class="pb-4 text-2xl text-slate-600">這裡是 app.vue 最外層</p>
    <NuxtLayout>
      <NuxtPage />
    </NuxtLayout>
  </div>

  <!-- Dynamic Import -->
    <div class="flex flex-col items-center">
    <div class="mt-8 flex items-center">
      <input
        id="show-button"
        v-model="show"
        name="show-button"
        type="checkbox"
        class="h-5 w-5"
      />
      <label for="show-button" class="ml-2 block text-base text-slate-800"
        >顯示報名按鈕</label
      >
    </div>
    <LazyBaseApplyButton v-if="show" />
  </div>


  <!-- NuxtLink for page changing -->
  <div class="my-4 flex justify-center gap-x-4">
    <nuxt-link to="/">Home</nuxt-link>
    <nuxt-link to="/about">About</nuxt-link>
    <nuxt-link to="/contact">Contact</nuxt-link>
    <nuxt-link to="/posts">posts</nuxt-link>
    <nuxt-link to="/docs">docs</nuxt-link>
    <nuxt-link to="/custom">custom</nuxt-link>
  </div>
</template>

<script setup>
const show = ref(false);
</script>

<style lang="scss" scoped></style>

