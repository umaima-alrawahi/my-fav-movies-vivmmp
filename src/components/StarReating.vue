<script setup>
const props = defineProps({score: Number})
const MARKER = '⭐';
</script>

<template>
  <span v-if="score >= 90">
      {{ MARKER }}{{ MARKER }}{{ MARKER }}{{ MARKER }}{{ MARKER }}
    </span>
    <span v-else-if="score >= 80">
      {{ MARKER }} {{ MARKER }} {{ MARKER }} {{ MARKER }}
    </span>
    <span v-else-if="score >= 60">
      {{ MARKER }} {{ MARKER }} {{ MARKER }}
    </span>
    <span v-else-if="score >= 40"> {{ MARKER }} {{ MARKER }} </span>
    <span v-else> {{ MARKER }}</span>
</template>
