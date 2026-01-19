<template>
  <footer class="bg-black/90 text-gray-400 py-16">
    <div class="max-w-7xl mx-auto px-4">
      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-10">
        <div>
          <div class="flex items-center gap-2 text-white text-2xl font-bold">
            <Logo />
          </div>
          <p class="text-sm mt-4 max-w-xs">
            Crafting exceptional coffee experiences since 2018.
          </p>
        </div>

        <div>
          <h3 class="text-white font-semibold mb-4">Explore</h3>
          <ul class="space-y-2 text-sm">
            <li><a href="#" class="hover:text-white">Our Menu</a></li>
            <li><a href="#" class="hover:text-white">Locations</a></li>
            <li><a href="#" class="hover:text-white">Our Store</a></li>
            <li><a href="#" class="hover:text-white">Careers</a></li>
          </ul>
        </div>

        <div>
          <h3 class="text-white font-semibold mb-4">Support</h3>
          <ul class="space-y-2 text-sm">
            <li><a href="#" class="hover:text-white">Contact Us</a></li>
            <li><a href="#" class="hover:text-white">FAQs</a></li>
            <li><a href="#" class="hover:text-white">Gift Cards</a></li>
            <li><a href="#" class="hover:text-white">Rewards</a></li>
          </ul>
        </div>

        <div>
          <h3 class="text-white font-semibold mb-4">Connect</h3>
          <div class="flex items-center gap-4">
            <IconInstagram
              class="h-10 w-10 p-2.5 text-white rounded-full bg-gray-500/30 hover:bg-gray-300/30 cursor-pointer"
            />

            <IconTwitter
              class="h-10 w-10 p-2.5 text-white rounded-full bg-gray-500/30 hover:bg-gray-300/30 cursor-pointer"
            />

            <IconFacebook
              class="h-10 w-10 p-2.5 text-white rounded-full bg-gray-500/30 hover:bg-gray-300/30 cursor-pointer"
            />
          </div>
        </div>
      </div>

      <div class="border-t border-gray-700 mt-12 pt-6 text-sm text-center">
        © 2024 Brewly Coffee. All rights reserved.
      </div>
    </div>
  </footer>
</template>
<script setup>
import Logo from "./Logo.vue";
import IconFacebook from "./IconFacebook.vue";
import IconTwitter from "./IconTwitter.vue";
import IconInstagram from "./IconInstagram.vue";
</script>
