<template>
  <div
    class="flex flex-col items-start gap-2 p-4.5 rounded-lg transition shadow-lg hover:shadow-sm bg-white border border-gray-200"
  >
    <div
      class="flex items-center justify-center p-2 rounded-lg bg-pumpkin-100/50"
    >
      <!-- Dynamicznie przekazany component ikony-->
      <component :is="icon" class="size-8 text-pumpkin-500" />
    </div>

    <div class="flex items-center justify-between w-full gap-2">
      <h3 class="text-lg font-semibold my-3">
        {{ title }}
      </h3>
      <slot name="badge" />
    </div>

    <p class="text-sm text-left text-gray-500 my-3">
      {{ desc }}
    </p>

    <div class="flex items-center justify-between w-full gap-2 mt-auto">
      <span class="text-2xl font-bold">{{ price }}</span>
      <Button label="Add" />
    </div>
  </div>
</template>
<script setup>
defineProps({
  icon: {
    type: Object,
  },
  title: String,
  desc: String,
  price: String,
});
import Badge from "./Badge.vue";
import Button from "./Button.vue";
</script>
