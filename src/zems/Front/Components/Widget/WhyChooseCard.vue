<script setup>
defineProps({
  item: {
    type: Object
  }
})
</script>
<template>
  <div class="why-choose-card relative all-4">
    <BaseImage :image="item.icon" />
    <div class="card-content span-3">
      <SubTitle>{{ item.title }}</SubTitle>
      <BaseParagraph>{{ item.description }}</BaseParagraph>
    </div>
  </div>
</template>
<style>
.why-choose-card {
  padding: 2.5rem 1.5rem;
  background: var(--white-color);
  box-shadow: var(--box-shadow);
  border-radius: .75rem;
}
.why-choose-card p {
  margin: .5rem 0 0 0;
}
.why-choose-card img {
  height: 60px;
  width: 60px;
}
</style>
