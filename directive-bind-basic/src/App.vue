<script setup lang="ts">
import { ref } from 'vue'

const url = ref('https://vuejs.org')
</script>

<template>
  <div>
    <!-- v-bindは要素の属性値をバインドする -->
    <p><a v-bind:href="url" target="_blank">Vue.jsのサイト</a></p>
    <p><a :href="url" target="_blank">Vue.jsのサイト（省略形）</a></p>
    <p>
      <a v-bind:href="url + 'guide/introduction.html'" target="_blank">Vue.jsのガイドのページ</a>
    </p>
  </div>
</template>