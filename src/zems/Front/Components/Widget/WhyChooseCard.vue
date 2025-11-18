<script setup>
defineProps({
  item: {
    type: Object
  }
})
</script>
<template>
  <div class="why-choose-card relative">
    <BaseImage class="mb-1" :image="item.image" />
    <SubTitle>{{ item.title }}</SubTitle>
    <BaseParagraph>{{ item.description }}</BaseParagraph>
  </div>
</template>
<style>
.why-choose-card {
  padding: 1rem;
  background: var(--white-color);
  box-shadow: var(--box-shadow);
  border-radius: .75rem;
}

.why-choose-card p {
  margin: .5rem 0 0 0;
}
.why-choose-card img {
  height: 240px;
  width: 100%;
  border-radius: .75rem .75rem 0 0;
}
</style>
