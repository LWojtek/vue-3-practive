<template>
  <div class="inline-flex items-center gap-1 px-2.5 py-1 rounded-full text-sm">
    <slot name="icon" />
    {{ label }}
  </div>
</template>
<script setup>
import { defineProps } from "vue";
defineProps({
  label: {
    type: String,
    default: "Badge",
  },
});
</script>
