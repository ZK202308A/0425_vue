
<script setup>

const props = defineProps(['arr'])

</script>

<template>

  <ul>
    <li v-for="todo in props.arr">
      {{todo}}
    </li>
  </ul>


</template>

<style scoped>

</style>