<script setup lang="ts">
import { ref } from 'vue'

const imgAttributes = ref({
  // assetの中は外部からは参照できないため、publicフォルダに配置する
  src: '/images/logo.svg',
  alt: 'VueLogo',
  width: '100',
  height: '100'
})
</script>

<template>
  <p><img v-bind="imgAttributes" /></p>
</template>