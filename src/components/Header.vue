<template>
  <header class="border-b border-gray-200 shadow-xs h-16">
    <div
      class="max-w-7xl px-2 sm:px-4 lg:px-6 mx-auto flex justify-between h-full items-center"
    >
      <Logo />

      <Nav />

      <!-- Przyciski -->
      <div class="flex items-center gap-3">
        <Button label="Sign in" variant="2" />
        <Button label="Order Now" />
      </div>
    </div>
  </header>
</template>
<script setup>
import Logo from "./Logo.vue";
import Nav from "./Nav.vue";
import Button from "./Button.vue";
</script>
