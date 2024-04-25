
<script setup>

const props = defineProps(['arr'])
const emits = defineEmits(['remove'])

const handleDelete = (tno) => {
  emits('remove', tno)
}

</script>

<template>

  <ul>
    <li v-for="todo in props.arr" :key=todo.tno>
      {{todo}}
      <button @click="() => handleDelete(todo.tno) ">X</button>
    </li>
  </ul>


</template>

<style scoped>

</style>