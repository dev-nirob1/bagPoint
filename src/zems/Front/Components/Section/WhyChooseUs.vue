<script setup>
import { ref } from 'vue';
import SectionTitle from '../Widget/SectionTitle.vue';
import WhyChooseCard from '../Widget/WhyChooseCard.vue';

const whyChooseUs = ref([
  {
    title: "Premium Quality",
    description: "Our bags are made from high-quality materials to last longer and withstand daily use.",
    icon: "https://img.icons8.com/color/48/000000/diamond.png"
  },
  {
    title: "Ergonomic Design",
    description: "Designed for comfort with padded straps and back support for all-day wear.",
    icon: "https://img.icons8.com/color/48/000000/diamond.png"
  },
  {
    title: "Multiple Compartments",
    description: "Keep all your essentials organized with designated compartments for laptop, books, and accessories.",
    icon: "https://img.icons8.com/color/48/000000/backpack.png"
  },
  {
    title: "Eco-Friendly",
    description: "Made with sustainable materials, helping you make an environmentally conscious choice.",
    icon: "https://img.icons8.com/color/48/000000/diamond.png"
  },
  {
    title: "Stylish & Trendy",
    description: "Modern designs and vibrant colors that match your style and personality.",
    icon: "https://img.icons8.com/color/48/000000/backpack.png"
  }
])
</script>

<template>
  <section class="why-choose-us">
    <div class="container">
      <div class="medium-2 large-3 gap-2">
        <SectionTitle class="py-1" title="Why Choose BagPoint?"
          subTitle="Stylish, durable, and designed for students who carry their world with them." />

        <WhyChooseCard v-for="(item, i) in whyChooseUs" :key="i" :item="item"/>
      </div>
    </div>
  </section>
</template>
<style scoped>
.why-choose-us {
  padding: 3.75rem 0;
}
</style>
