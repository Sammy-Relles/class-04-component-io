<script setup>
defineProps({
  increment: Number
})
defineEmits(['increase-by'])
</script>

<template>
  <div class="component">
    <button v-on:click="$emit('increase-by', increment)">Increase Count</button>
  </div>
</template>

<style scoped>
.component {
  background-color: lightsteelblue;
  padding: 1rem;
}
</style>
