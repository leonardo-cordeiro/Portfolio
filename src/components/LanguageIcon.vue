<template>
  <div class="language-icon">
    <img :src="icon" :alt="alt" />
  </div>
</template>

<script setup>
defineProps({
  icon: String,
  alt: String
})
</script>

<style scoped>
.language-icon img {
  margin-right: 5px;
  width: 40px;
  height: 40px;
  cursor: pointer;
  transition:
    width 1s,
    height 1s;
}

.language-icon img:hover {
  width: 50px;
  height: 50px;
}
</style>
