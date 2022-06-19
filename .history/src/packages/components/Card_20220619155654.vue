<template>
  <div class="my-card">
    <div class="card-header">{{ title }}</div>
    <div class="card-body">{{ content }}</div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue'
defineProps<{
  title: string
  content: string
}>()
</script>

<style scoped lang="less">
.my-card {
  width: 300px;
  height: 300px;
  .card-header {
    height: 60px;
    line-height: 60px;
    border-bottom: 1px solid rgb(121, 119, 119, 0.2);
    font-size: 14px;
    font-weight: 600;
    text-align: center;
  }
  .card-body {
    font-size: 14px;
    color: #666;
    padding: 10px;
  }
}
</style>
