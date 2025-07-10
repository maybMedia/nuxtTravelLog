<script setup lang="ts">
import AuthButton from "~/components/auth-button.vue";
</script>

<template>
  <div class="hero bg-base-300 container mx-auto my-4">
    <div class="hero-content text-center min-h-96">
      <div class="max-w-md">
        <h1 class="text-5xl font-bold">
          Hey there,
        </h1>
        <p class="py-6">
          Save your travel memories with Travel Logger, the app that helps you document your journeys and share them with friends and family.
        </p>
        <AuthButton />
      </div>
    </div>
  </div>
</template>
