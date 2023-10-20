<script setup lang="ts">
import { ref } from 'vue'

const widthOrHeight = ref('height')
const widthOrHeightValue = ref('100')
</script>

<template>
  <div>
    <p>
      <!-- 動的引数 -->
      <img alt="VueLogo" src="./assets/logo.svg" v-bind:[widthOrHeight]="widthOrHeightValue" />
    </p>
  </div>