<template>
  <NuxtLink
    :to="to"
    class="text-base font-medium text-gray-500 hover:text-gray-900"
  >
    {{ title }}
  </NuxtLink>
</template>

<script setup>
const props = defineProps({
  to: String,
  title: String,
});
</script>
