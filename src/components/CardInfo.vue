<template>
  <div class="flex flex-col gap-2 p-4">
    <div
      class="flex items-center justify-center p-3 rounded-full bg-pumpkin-100/50 mx-auto"
    >
      <component :is="icon" class="size-8 text-pumpkin-500" />
    </div>

    <h3 class="text-xl font-semibold my-3 text-center">
      {{ title }}
    </h3>

    <p class="text-base text-gray-500">
      {{ desc }}
    </p>
  </div>
</template>
<script setup>
defineProps({
  icon: {
    type: Object,
  },
  title: String,
  desc: String,
});
</script>
