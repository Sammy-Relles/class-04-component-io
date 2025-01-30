<script setup>
import IncreaseCount from './components/IncreaseCount.vue'
import ShowCount from './components/ShowCount.vue'
</script>

<template>
  <div class="component">
    <ShowCount />
    <IncreaseCount />
  </div>
</template>

<style scoped>
.component>* {
  margin-bottom: 1rem;
}
</style>
