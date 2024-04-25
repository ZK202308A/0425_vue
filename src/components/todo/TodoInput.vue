<script setup>

import {ref} from "vue";

const emits = defineEmits(['add'])
const text = ref('Hello')

const handleClick = () => {
  emits('add', text.value)
}

</script>

<template>
  <input type="text" v-model=text>
  <button @click=handleClick >SAVE</button>
</template>

<style scoped>

</style>