<template>
  <!-- Variant 1-->
  <button
    v-if="variant === '1'"
    class="inline-flex gap-2 items-center bg-pumpkin-500 disabled:opacity-50 disabled:cursor-not-allowed rounded-md cursor-pointer transition duration-200 shadow-md not-disabled:hover:shadow-lg border-2 border-pumpkin-500 not-disabled:hover:border-pumpkin-500/80 focus-visible:outline-2 outline-offset-2 focus-visible:outline-pumpkin-500 not-disabled:hover:bg-pumpkin-500/80 text-white"
    :class="[size === 'md' ? ' py-1.5 px-4 text-sm' : 'py-3 px-6 text-lg']"
  >
    {{ label }}
    <svg
      v-if="showIcon"
      xmlns="http://www.w3.org/2000/svg"
      viewBox="0 0 24 24"
      fill="none"
      stroke="currentColor"
      stroke-width="2"
      stroke-linecap="round"
      stroke-linejoin="round"
      class="size-5"
    >
      <path d="M5 12h14" />
      <path d="m12 5 7 7-7 7" />
    </svg>
  </button>

  <!-- Variant 2-->
  <button
    v-if="variant === '2'"
    class="inline-flex gap-2 items-center disabled:opacity-50 disabled:cursor-not-allowed rounded-md cursor-pointer transition duration-200 focus-visible:outline-2 outline-offset-2 focus-visible:outline-black not-disabled:hover:bg-gray-100 py-1.5 px-4"
    :class="[size === 'md' ? ' py-1.5 px-4 text-sm' : 'py-3 px-6 text-lg']"
  >
    {{ label }}
    <svg
      v-if="showIcon"
      xmlns="http://www.w3.org/2000/svg"
      viewBox="0 0 24 24"
      fill="none"
      stroke="currentColor"
      stroke-width="2"
      stroke-linecap="round"
      stroke-linejoin="round"
      class="size-5"
    >
      <path d="M5 12h14" />
      <path d="m12 5 7 7-7 7" />
    </svg>
  </button>

  <!-- Variant 3-->
  <button
    v-if="variant === '3'"
    class="inline-flex gap-2 items-center disabled:opacity-50 disabled:cursor-not-allowed border-2 border-gray-200 rounded-md cursor-pointer transition duration-200 focus-visible:outline-2 outline-offset-2 focus-visible:outline-gray-500 not-disabled:hover:bg-gray-200 not-disabled:hover:border-amber-500/30 py-1.5 px-4"
    :class="[size === 'md' ? ' py-1.5 px-4 text-sm' : 'py-3 px-6 text-lg']"
  >
    {{ label }}
    <svg
      v-if="showIcon"
      xmlns="http://www.w3.org/2000/svg"
      viewBox="0 0 24 24"
      fill="none"
      stroke="currentColor"
      stroke-width="2"
      stroke-linecap="round"
      stroke-linejoin="round"
      class="size-5"
    >
      <path d="M5 12h14" />
      <path d="m12 5 7 7-7 7" />
    </svg>
  </button>
  <!-- Variant 4 -->
  <button
    v-if="variant === '4'"
    class="w-full flex justify-center gap-2 items-center bg-pumpkin-500 disabled:opacity-50 disabled:cursor-not-allowed rounded-md cursor-pointer transition duration-250 shadow-md not-disabled:hover:shadow-lg border-2 border-pumpkin-500 not-disabled:hover:border-pumpkin-500/80 focus-visible:outline-2 outline-offset-2 focus-visible:outline-pumpkin-500 not-disabled:hover:bg-pumpkin-500/80 active:scale-95 text-white"
    :class="[size === 'md' ? ' py-1.5 px-4 text-sm' : 'py-3 px-6 text-lg']"
  >
    {{ label }}
    <svg
      v-if="showIcon"
      xmlns="http://www.w3.org/2000/svg"
      viewBox="0 0 24 24"
      fill="none"
      stroke="currentColor"
      stroke-width="2"
      stroke-linecap="round"
      stroke-linejoin="round"
      class="size-5"
    >
      <path d="M5 12h14" />
      <path d="m12 5 7 7-7 7" />
    </svg>
  </button>
</template>

<script setup>
const props = defineProps({
  variant: {
    type: [String, Number],
    default: "1",
  },
  size: {
    type: String,
    default: "md",
  },
  showIcon: {
    type: Boolean,
    default: false,
  },
  label: String,
});
</script>
