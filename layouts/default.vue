<script lang="ts" setup>
const authStore = useAuthStore();
await authStore.init();
</script>

<template>
  <div class="min-h-screen flex flex-col">
    <AppNavBar />
    <main class="flex-1 flex flex-col">
      <slot />
    </main>
  </div>
</template>
