<script setup>

import {ref} from "vue";

const emits = defineEmits(['add'])
const text = ref('Hello')

</script>

<template>
  <input type="text" v-model=text>
  <button>SAVE</button>
</template>

<style scoped>

</style>