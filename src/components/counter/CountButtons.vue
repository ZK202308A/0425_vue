<script setup>

const emits = defineEmits(['doRun'])

const handleClick = (amount) => {
  emits('doRun', amount)
}

</script>

<template>
  <div>
    <button @click="() => handleClick(1)">INC</button>
    <button @click="() => handleClick(-1)">DEC</button>
  </div>
</template>

<style scoped>

</style>