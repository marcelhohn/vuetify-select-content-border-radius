<template>
  <v-select
    v-model="favorites"
    hint="Pick your favorite states"
    :items="states"
    label="Select"
    multiple
    persistent-hint
  />
</template>

<script setup>
  import { shallowRef } from 'vue'

  const favorites = shallowRef([])

  const states = [
    'Alabama',
    'Alaska',
    'American Samoa',
    'Arizona',
    'Arkansas',
    'California',
  ]
</script>
