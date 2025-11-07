<script setup>
import { ref } from 'vue';
import SectionTitle from '../Widget/SectionTitle.vue';
const features = ref([
  {
    id: 1,
    title: "Waterproof Fabric Shield Your Gear",
    description: "Repels rain and spills so your essentials stay dry no matter the weather.",
    icon: "fa-solid fa-droplet-slash",
    image: "https://images.unsplash.com/photo-1611010344444-5f9e4d86a6e1?ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&q=80&w=464",
  },
  {
    id: 2,
    title: "Anti Theft Pocket",
    description: "Hidden zipper pocket keeps your valuables safe during travel or commute.",
    icon: "fa-solid fa-lock",
    image: "https://images.unsplash.com/photo-1667411425122-8b6be5da1c48?ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&q=80&w=870",
  },
  {
    id: 3,
    title: "Laptop Compartment",
    description: "Padded straps and breathable mesh backing for effortless carrying all day long.",
    icon: "fa-solid fa-house-laptop",
    image: "https://images.unsplash.com/photo-1650500426868-27a68714a4a4?ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&q=80&w=387",
  },
  {
    id: 4,
    title: "Ergonomic Design",
    description: "Comfort Engineered For Long Days and Longer Journeys",
    icon: "fa-solid fa-feather",
    image: "https://images.unsplash.com/photo-1544141161-30fef2b4ba6a?ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&q=80&w=465",
  },
  {
    id: 5,
    title: "LightWeight And Durable",
    description: "Performance Without Compromise, Built To Last.",
    icon: "fa-solid fa-user-shield",
    image: "https://images.unsplash.com/photo-1625060371499-8a01616c86f0?ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxzZWFyY2h8MTI0fHxlcmdvbm9taWMlMjBkZXNpZ24lMjBiYWd8ZW58MHx8MHx8fDA%3D&auto=format&fit=crop&q=60&w=500",
  }
])
</script>

<template>
  <section class="features">

    <div class="container">
      <SectionTitle class="text-center mb-3" title="Built For Every Journey"
        subTitle="Precision engineering meets everyday functionality." />

      <div class="medium-2 large-4 gap-2">
        <div v-for="(item, i) in features" :key="i" class="feature-card">
          <i :class="item.icon" class="fa-2x mb-1"></i>
          <BaseTitle>{{ item.title }}</BaseTitle>
          <BaseParagraph>{{ item.description }}</BaseParagraph>
          <BaseImage :image="item.image" />
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.features {
  padding: 3.75rem 0;
}

.feature-card {
  position: relative;
  padding: 1.5rem;
  box-shadow: var(--box-shadow);
  color: var(--white-color);
  border-radius: .75rem;
  background: linear-gradient(to bottom, rgba(0, 0, 0, .4), rgba(0, 0, 0, .3))
}

.feature-card:nth-child(1) {
  grid-column: 1 / span 2;
  grid-row: 1 / span 2;
  place-content: center;
}

.feature-card img {
  position: absolute;
  inset: 0;
  width: 100%;
  height: 100%;
  z-index: -1;
  border-radius: .75rem;
}
</style>
