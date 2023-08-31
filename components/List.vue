<template>
  <ul class="list">
    <slot></slot>
  </ul>
</template>

<script setup>
import { ref } from 'vue';

const count = ref(0);
</script>

<style lang="scss" scoped>
.list {
  margin: 0;
  padding: 0;

  > li + li {
    margin-top: 16px;
  }
}
</style>
