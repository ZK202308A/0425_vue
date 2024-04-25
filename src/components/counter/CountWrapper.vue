<script setup>

import CountDisplay from "./CountDisplay.vue";
import CountButtons from "./CountButtons.vue";
import {ref} from "vue";

const data = ref(3)
</script>

<template>
  <CountDisplay :num=data />
  <CountButtons/>
</template>

<style scoped>

</style>