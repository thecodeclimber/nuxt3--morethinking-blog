<template>
  <div class="-my-2 -mr-2 md:hidden">
    <PopoverButton
      class="inline-flex items-center justify-center rounded-md bg-white p-2 text-gray-400 hover:bg-gray-100 hover:text-gray-500 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-indigo-500"
    >
      <span class="sr-only">Open menu</span>
      <MenuIcon class="h-6 w-6" aria-hidden="true" />
    </PopoverButton>
  </div>
</template>

<script setup>
import { PopoverButton } from "@headlessui/vue";

import { MenuIcon } from "@heroicons/vue/outline";
</script>
