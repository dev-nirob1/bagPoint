<script setup>
import { ref } from 'vue';
import SectionTitle from '../Widget/SectionTitle.vue';
import WhyChooseCard from '../Widget/WhyChooseCard.vue';
const whyChooseUs = ref([
  {
    title: "Premium Materials",
    description: "Crafted from durable, water-resistant fabric that lasts longer and protects your essentials.",
    image: "https://images.unsplash.com/photo-1578753557366-92159d4c8a11?q=80&w=1470&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
  },
  {
    title: "All-Day Comfort",
    description: "Ergonomic, cushioned straps designed to reduce shoulder strain during long days.",
    image: "https://images.unsplash.com/photo-1681334921939-02af23b28b81?q=80&w=387&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
  },
  {
    title: "Smart Organization",
    description: "Dedicated compartments for your laptop, books, accessories, and bottles.",
    image: "https://images.unsplash.com/photo-1623137433874-9bdf8eb442bc?q=80&w=871&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
  },
{
  title: "Lightweight Design",
  description: "Carry more with less effort thanks to a lightweight yet durable build.",
  image: "https://images.unsplash.com/photo-1595724281096-bd3e2b66c86a?q=80&w=870&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
},
  {
    title: "Modern & Stylish",
    description: "Minimalist design that fits school, travel, work, and everyday life.",
    image: "https://images.unsplash.com/photo-1681334921914-df210bc8083a?q=80&w=387&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
  },
  {
  title: "Water-Resistant Protection",
  description: "Keeps your essentials safe from rain and accidental spills with a water-repellent exterior.",
  image: "https://images.unsplash.com/photo-1578753557366-92159d4c8a11?q=80&w=1470&auto=format&fit=crop&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D"
}
])

</script>

<template>
  <section class="why-choose-us">
    <div class="container">
      <SectionTitle class="mb-2 text-center" title="Why Choose BagPoint?"
        subTitle="Stylish, durable, and designed for students who carry their world with them." />

      <div class="medium-2 large-3 gap-2">
        <WhyChooseCard v-for="(item, i) in whyChooseUs" :key="i" :item="item" />
      </div>
    </div>
  </section>
</template>
<style scoped>
.why-choose-us {
  padding: 3.75rem 0;
}
</style>
