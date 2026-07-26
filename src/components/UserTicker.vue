<template>
  <div class="glass-card ticker-card">
    <div class="ticker-wrapper">
      <div v-for="(item, index) in tickerItems" :key="index" class="ticker-item">
        <span>{{ item.text }}</span>
        <span style="color: var(--success-color); font-weight: bold;">[生成完成]</span>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref } from 'vue';

const tickerItems = ref([
  {
    "text": "用户 135****8801 完成了月收入 8000 元的 532 存钱预算规划"
  },
  {
    "text": "用户 189****2239 生成了月光族外卖与冲动购物止血诊断报告"
  },
  {
    "text": "用户 131****6610 完成了首年攒下 3 万元无痛储蓄计划"
  },
  {
    "text": "用户 158****4492 生成了三口之家月度固定开支优化方案"
  },
  {
    "text": "用户 173****5509 分析了信用卡账单并规划了半年清偿路径"
  }
]);
</script>
