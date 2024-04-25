
<script setup>

const props = defineProps(['arr'])

</script>

<template>

  <ul>
    <li v-for="todo in props.arr" :key=todo.tno>
      {{todo}}
    </li>
  </ul>


</template>

<style scoped>

</style>