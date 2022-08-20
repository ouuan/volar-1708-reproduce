<template>
  {{ depth }}
  <recursive-component v-if="depth > 0" :depth="depth - 1"/>
</template>

<script setup lang="ts">
defineProps<{ depth: number }>();
</script>
