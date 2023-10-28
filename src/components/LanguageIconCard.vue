<template>
  <ToolTip flow="down" :tooltip="alt">
    <div class="language-icon">
      <img :src="icon" :alt="alt" />
    </div>
  </ToolTip>
</template>

<script setup>
import ToolTip from '@/components/ToolTip.vue'
defineProps({
  icon: String,
  alt: String
})
</script>

<style scoped>
.language-icon img {
  width: 60px;
  height: 60px;
  object-fit: cover;
  border-radius: 10px;
  margin: 0 15px;
  background: #fffdfd82;
  cursor: pointer;
  z-index: 1;
}
</style>
