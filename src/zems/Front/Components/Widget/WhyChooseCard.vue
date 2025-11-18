<script setup>
defineProps({
  item: {
    type: Object
  }
})
</script>
<template>
  <div class="why-choose-card relative">
    <div class="image mb-1">
      <BaseImage :image="item.image" />
    </div>
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
  cursor: pointer;
}

.why-choose-card p {
  margin: .5rem 0 0 0;
}
.why-choose-card .image{
  height: 240px;
  overflow:hidden;
  border-radius: .75rem .75rem 0 0;
}
.why-choose-card img {
  border-radius: .75rem .75rem 0 0;
  transition: all .5s ease-in-out;
}
.why-choose-card:hover img {
  transform: scale(1.1)
}
</style>
