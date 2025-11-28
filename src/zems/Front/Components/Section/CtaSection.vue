<script setup>
defineProps({
  handleOpenFormModal: {
    type: Function
  }
})
</script>

<template>
  <section class="cta bg-primary flex-center">
    <div class="cta-content">
      <BaseTitle>READY TO OWN THE PERFECT BAG</BaseTitle>
      <BaseParagraph>One back pack that adapts to your lifestyle, built for performance and comfort</BaseParagraph>
      <BaseButton @click="handleOpenFormModal" class="bg-secondary">Buy Now</BaseButton>
    </div>
  </section>
</template>
<style scoped>
.cta {
  padding: 8rem 0;
  text-align: center;
  color: var(--white-color);
}
.outline-btn {
  background: var(--dark-color);

}
.outline-btn:hover {
  background: var(--transparent-color);
}

</style>
