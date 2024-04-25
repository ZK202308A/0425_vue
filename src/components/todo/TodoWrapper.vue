<script setup>
import TodoList from "./TodoList.vue";
import {ref} from "vue";
import TodoInput from "./TodoInput.vue";

const todos = ref([
  {tno:1, title:'T1', complete:false},
  {tno:2, title:'T2', complete:false},
])

let sequence = 3

const addTodo = (title) => {

  const newTodo = {tno:sequence++, title:title, complete: false }

  todos.value.push(newTodo)
}

const removeTodo = (tno) => {

  todos.value = todos.value.filter(todo => todo.tno !== tno)

}





</script>

<template>
  <TodoInput @add=addTodo></TodoInput>
  <TodoList :arr="todos" @remove=removeTodo></TodoList>

</template>

<style scoped>

</style>