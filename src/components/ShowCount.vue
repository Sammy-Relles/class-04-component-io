<script setup>
defineProps({
  count: Number
})
</script>

<template>
  <div class="component">
    <p>Count: {{count}}</p>
  </div>
</template>

<style scoped>
.component {
  background-color: papayawhip;
  padding: 1rem;
}
</style>
