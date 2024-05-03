<template>
  <v-row justify="center">
    <v-col cols="10" md="6">
      <!--eslint-disable-next-line vue/no-mutating-props-->
      <v-text-field :label="'Número ' + props.position" v-model="props.n"> </v-text-field>
      <v-text-field label="Tipo do valor" readonly v-model="nType"> </v-text-field>
    </v-col>
  </v-row>
</template>

<script setup lang="ts">
const props = defineProps({
  n: Number,
  position: Number
})
const nType = typeof props.n
</script>
