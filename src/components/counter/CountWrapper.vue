<script setup>

import CountDisplay from "./CountDisplay.vue";
import CountButtons from "./CountButtons.vue";
import {ref} from "vue";

const data = ref(3)

const change = (amount) => {
  data.value += amount
}


</script>

<template>
  <CountDisplay :num=data />
  <CountButtons @doRun=change />
</template>

<style scoped>

</style>