<template>
  <v-container-fluid>
    <VInputNumber :n="n1" :position="addCount()" />
    <VInputNumber :n="n2" :position="addCount()" />
  </v-container-fluid>
</template>

<script setup lang="ts">
import VInputNumber from './VInputNumber.vue'
const n1 = 'Olá'
const n2 = 10
let i = 0
const addCount = () => {
  return i++
}
</script>
