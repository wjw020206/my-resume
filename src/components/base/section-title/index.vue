<template>
  <div class="section-title">{{ title }}</div>
</template>

<script setup lang="ts">
defineProps<{
  title: string
}>()
</script>

<style lang="scss" scoped>
.section-title {
  color: #000;
  text-align: start;
  border-bottom: 2px solid #000;
  margin: 8px 0 4px;
  font-size: 18px;
  font-weight: 600;
  line-height: 32px;
}
</style>
