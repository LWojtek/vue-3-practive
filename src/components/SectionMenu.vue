<template>
  <section id="menu" class="py-24 bg-gray-100/30">
    <div
      class="max-w-7xl text-center px-2 sm:px-4 lg:px-6 mx-auto flex justify-center items-center"
    >
      <div class="flex flex-col items-center gap-8 flex-grow">
        <Badge label="Our menu" class="bg-gray-100 border border-gray-300" />
        <h2 class="text-5xl font-bold">Crafted with Love</h2>
        <p>
          From our signature espresso blends to freshly baked treats, every item
          is made with care.
        </p>

        <div
          class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-6 w-full my-12"
        >
          <Card
            :icon="IconCoffee"
            title="Classic Espresso"
            desc="Rich, bold, and perfectly balanced with notes of dark chocolate."
            price="$4.50"
          >
            <template #badge>
              <Badge label="Bestseller" class="bg-pumpkin-500 text-white" />
            </template>
          </Card>
          <Card
            :icon="IconLeaf"
            title="Oat Milk Latte"
            desc="Smooth espresso with creamy oat milk and a hint of vanilla."
            price="$5.50"
          >
            <template #badge>
              <Badge label="Vegan" class="bg-green-600 text-white" />
            </template>
          </Card>
          <Card
            :icon="IconCroissant"
            title="Butter Croissant"
            desc="Flaky, golden layers of French-style pastry perfection."
            price="$3.75"
          >
            <template #badge>
              <Badge label="Fresh Daily" class="bg-yellow-500 text-black" />
            </template>
          </Card>
          <Card
            :icon="IconIceCream"
            title="Affogatto"
            desc="Vanilla gelato drowned in a shot of hot espresso."
            price="$6.00"
          >
            <template #badge>
              <Badge label="Seasonal" class="bg-blue-400 text-white" />
            </template>
          </Card>
        </div>
        <Button label="View Full Menu" size="lg" variant="3" />
      </div>
    </div>
  </section>
</template>

<script setup>
import Badge from "./Badge.vue";
import Button from "./Button.vue";
import Card from "./Card.vue";

import IconCoffee from "./IconCoffee.vue";
import IconLeaf from "./IconLeaf.vue";
import IconCroissant from "./IconCroissant.vue";
import IconIceCream from "./IconIceCream.vue";
</script>
