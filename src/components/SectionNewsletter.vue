<template>
  <section class="bg-pumpkin-100/30 py-24">
    <div class="max-w-7xl mx-auto px-2 flex justify-center">
      <div
        class="flex flex-col items-center bg-white shadow-xl rounded-lg p-12 gap-6 w-full md:w-2/3 lg:w-1/2"
      >
        <div class="bg-pumpkin-100/50 p-4 rounded-full">
          <component :is="IconGift" class="h-8 w-8 text-pumpkin-500" />
        </div>

        <h2 class="text-3xl md:text-4xl font-bold text-center">
          Get 20% Off Your First Order
        </h2>

        <p class="text-base text-gray-500 text-center">
          Join our newsletter and receive exclusive offers, new menu alerts, and
          a welcome discount.
        </p>

        <div class="relative w-full">
          <div
            class="absolute inset-y-0 left-3 flex items-center pointer-events-none"
          >
            <component :is="IconMail" class="h-5 w-5 text-gray-400" />
          </div>

          <input
            type="email"
            placeholder="Enter your email address"
            class="w-full pl-10 pr-4 py-3 rounded-lg border border-gray-300 text-base bg-gray-50 text-gray-700 placeholder-gray-400 focus:outline-none focus:ring-2 focus:ring-pumpkin-500 focus:ring-offset-2 focus:ring-offset-white"
          />
        </div>

        <label
          class="flex items-center gap-2 text-sm text-gray-500 w-full cursor-pointer"
        >
          <input
            type="checkbox"
            class="h-4 w-4 rounded border-2 border-gray-400 bg-white cursor-pointer checked:bg-pumpkin-500 checked:border-pumpkin-500 accent-white"
          />
          <span>
            I agree to receive promotional emails. You can unsubscribe at any
            time.
          </span>
        </label>

        <Button
          label="Subscribe & Get Discount"
          size="lg"
          variant="4"
          class="px-auto"
        />
      </div>
    </div>
  </section>
</template>

<script setup>
import IconMail from "./IconMail.vue";
import IconGift from "./IconGift.vue";
import Button from "./Button.vue";
</script>
