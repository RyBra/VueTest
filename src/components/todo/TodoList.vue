<template>
  <div class="todos">
    <Todo v-for="todo in todos" v-bind:todo="todo" v-bind:key="todo._id" />
  </div>
</template>


<script>
import Todo from "./Todo.vue";

export default {
  name: "TodoList",
  props: {
    todos: Object
  },
  components: {
    Todo
  }
};
</script>

<style>
.todos {
  margin: 0 auto;
  max-width: 768px;
}
</style>
