<script setup lang="ts">
import { ref } from 'vue'

const mousePointX = ref(0)
const mousePointY = ref(0)

const onMousemove = (event: MouseEvent): void => {
  mousePointX.value = event.clientX
  mousePointY.value = event.clientY
}
</script>

<template>
  <section>
    <img src="public/logo.svg" alt="Vueのロゴ" width="200" v-on:mousemove="onMousemove" />
    <p>ポイントの位置: x={{ mousePointerX }}; y={{ mousePointerY }}</p>
  </section>
</template>
