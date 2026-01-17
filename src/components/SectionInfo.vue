<template>
  <section class="bg-white/75 py-24">
    <div
      class="max-w-7xl text-center px-2 sm:px-4 lg:px-6 mx-auto flex justify-center items-center"
    >
      <div class="flex flex-col items-center gap-8 flex-grow">
        <Badge label="Why Choose Us" class="bg-blue-400 text-white" />
        <h2 class="text-5xl font-bold">More Than Just Coffee</h2>
        <p class="text-lg">
          We create experiences, not just beverages. Here's what makes us
          special.
        </p>

        <div
          class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6 w-full my-12"
        >
          <card-info
            :icon="IconMapPin"
            title="Prime Locations"
            desc="Find us in the heart of the city, always close to where you need us."
          >
          </card-info>
          <card-info
            :icon="IconClock"
            title="Open Early"
            desc="We're here from 6 AM, ready to kickstart your morning right."
          >
          </card-info>
          <card-info
            :icon="IconWifi"
            title="Free WiFi"
            desc="Stay connected while you sip. Perfect for remote work"
          >
          </card-info>
          <card-info
            :icon="IconHeart"
            title="Made with Love"
            desc="Every cup is crafted by passionate baristas who love what they do."
          >
          </card-info>
        </div>
      </div>
    </div>
  </section>
</template>
<script setup>
import Badge from "./Badge.vue";
import IconMapPin from "./IconMapPin.vue";
import IconClock from "./IconClock.vue";
import IconWifi from "./IconWifi.vue";
import IconHeart from "./IconHeart.vue";
import CardInfo from "./CardInfo.vue";
</script>
