<script setup>
import TodoList from "./TodoList.vue";
import {ref} from "vue";

const todos = ref([
  {tno:1, title:'T1', complete:false},
  {tno:2, title:'T2', complete:false},
])



</script>

<template>
  <TodoList :arr="todos"></TodoList>

</template>

<style scoped>

</style>