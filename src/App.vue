<template>
  <v-container-fluid>
    <v-row justify="center">
      <v-col cols="12" md="6">
        <v-switch label="Trocar para componente com TS" v-model="ts" color="info"></v-switch>
      </v-col>
    </v-row>
  </v-container-fluid>
  <UseWithTs v-if="ts"></UseWithTs>
  <UseWithJs v-else></UseWithJs>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import UseWithJs from '@/components/UseWithJs.vue'
import UseWithTs from '@/components/UseWithTs.vue'
const ts = ref(false)
</script>

<style lang="scss">
body {
  background-color: rgba(25, 25, 25);
  color: white;
  font-weight: bold;
  padding: 50px 0px;
}
</style>
