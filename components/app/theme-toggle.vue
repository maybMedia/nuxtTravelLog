<script setup lang="ts">
const colorMode = useColorMode();

const isDark = computed({
  get() {
    return colorMode.value === "dark";
  },
  set(value) {
    colorMode.preference = value ? "dark" : "light";
  },
});
</script>

<template>
  <label class="swap swap-rotate mx-4">
    <input v-model="isDark" type="checkbox">
    <Icon name="tabler:sun-filled" class="swap-on" size="24" style="color: hsl(173, 100%, 41%)" />
    <Icon name="tabler:moon-filled" class="swap-off" size="24" style="color: hsl(173, 100%, 41%)" />
  </label>
</template>
