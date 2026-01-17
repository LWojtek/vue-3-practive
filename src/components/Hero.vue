<template>
  <section
    class="flex items-stretch relative h-[calc(100vh-var(--header-height))]"
  >
    <!-- BG -->
    <div
      class="pointer-events-none absolute inset-0 bg-gradient-to-br from-pumpkin-500/10 via-background to-blue-500/5"
    />
    <div
      class="pointer-events-none absolute top-20 right-20 w-72 h-72 bg-pumpkin-500/10 rounded-full blur-3xl"
    />
    <div
      class="pointer-events-none absolute bottom-20 left-20 w-96 h-96 bg-blue-500/10 rounded-full blur-3xl"
    />

    <!-- Content -->
    <div
      class="max-w-7xl text-center px-2 sm:px-4 lg:px-6 mx-auto flex items-center"
    >
      <div class="flex flex-col items-center gap-12">
        <Badge label="Artisan Coffee Since 2018" class="bg-gray-200">
          <template #icon
            ><svg
              xmlns="http://www.w3.org/2000/svg"
              viewBox="0 0 24 24"
              fill="none"
              stroke="currentColor"
              stroke-width="2"
              stroke-linecap="round"
              stroke-linejoin="round"
              class="size-4"
            >
              <path d="M10 2v2" />
              <path d="M14 2v2" />
              <path
                d="M16 8a1 1 0 0 1 1 1v8a4 4 0 0 1-4 4H7a4 4 0 0 1-4-4V9a1 1 0 0 1 1-1h14a4 4 0 1 1 0 8h-1"
              />
              <path d="M6 2v2" />
            </svg>
          </template>
        </Badge>

        <h1 class="text-7xl font-bold max-w-[13ch]">
          Where Every Cup Tells a <span class="text-pumpkin-500">Story</span>
        </h1>

        <p class="text-xl text-gray-500 max-w-[45ch]">
          Handcrafted specialty coffee, freshly baked goods, and a warm
          atmosphere to fuel your day.
        </p>

        <div class="flex items-center gap-4">
          <Button size="lg" label="View Our Menu" show-icon />
          <Button size="lg" variant="3" label="Find a Location" />
        </div>
      </div>
    </div>
  </section>
</template>
<script setup>
import Button from "./Button.vue";
import Badge from "./Badge.vue";
</script>
