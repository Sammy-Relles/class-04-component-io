<script setup>
import IncreaseCount from './components/IncreaseCount.vue'
import ShowCount from './components/ShowCount.vue'
import { ref } from 'vue'

const c = ref(0)

function increaseCount(inc) {
  c.value = c.value + Number(inc)
}
</script>

<template>
  <div class="component">
    <ShowCount v-bind:count="c" />
    <IncreaseCount increment="1"
    v-on:increase-by="increaseCount"/>
    <IncreaseCount increment="10"
    v-on:increase-by="increaseCount"/>
    <IncreaseCount increment="100"
    v-on:increase-by="increaseCount"/>
    <!-- a reusable component to call -->
  </div>
</template>

<style scoped>
.component>* {
  margin-bottom: 1rem;
}
</style>
