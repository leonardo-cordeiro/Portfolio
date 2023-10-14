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
  margin-right: 5px;
  width: 35px;
  height: 35px;
  cursor: pointer;
}
</style>
