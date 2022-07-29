<template>
  <transition
    enter-active-class="duration-200 ease-out"
    enter-from-class="opacity-0 scale-95"
    enter-to-class="opacity-100 scale-100"
    leave-active-class="duration-100 ease-in"
    leave-from-class="opacity-100 scale-100"
    leave-to-class="opacity-0 scale-95"
  >
    <PopoverPanel
      focus
      class="absolute inset-x-0 top-0 origin-top-right transform p-2 transition md:hidden"
    >
      <div
        class="divide-y-2 divide-gray-50 rounded-lg bg-white shadow-lg ring-1 ring-black ring-opacity-5"
      >
        <slot />
      </div>
    </PopoverPanel>
  </transition>
</template>

<script setup>
import { PopoverPanel } from "@headlessui/vue";
</script>
