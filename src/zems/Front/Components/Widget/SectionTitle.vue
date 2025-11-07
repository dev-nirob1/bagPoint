<script setup>
defineProps({
  title: {
    type: String
  },
  subTitle: {
    type: String
  }
})
</script>
<template>
  <div class="section-title">
    <BaseTitle>{{ title }}</BaseTitle>
    <BaseParagraph>{{ subTitle }}</BaseParagraph>
  </div>
</template>
<style>
.section-title p{
  margin: .5rem 0;
}</style>
