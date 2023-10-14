<template>
  <Tooltip flow="down" :tooltip="alt">
    <div class="language-icon">
      <img :src="icon" :alt="alt" />
    </div>
  </Tooltip>
</template>

<script setup>
import Tooltip from '@/components/Tooltip.vue'
defineProps({
  icon: String,
  alt: String
})
</script>

<style scoped>
.language-icon img {
  margin-right: 5px;
  width: 35px;
  height: 35px;
  cursor: pointer;
}
</style>
