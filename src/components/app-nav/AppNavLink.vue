<script setup lang="ts">
const props = defineProps({
  link: { type: String, required: true },
});
</script>

<template>
  <router-link :to="props.link" class="w-full hover:bg-light-secondary dark:hover:bg-dark-secondary">
    <div class="flex flex-row items-center justify-center text-left p-4 w-full">
      <slot></slot>
    </div>
  </router-link>
</template>
