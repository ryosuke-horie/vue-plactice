<script setup lang="ts">
import { ref } from 'vue'

const isButtonDisabled = ref(true)
</script>

<template>
  <div>
    <p><button type="button" v-bind:disabled="isButtonDisabled">送信</button></p>
  </div>
</template>