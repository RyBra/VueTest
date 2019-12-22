<template>
  <div class="todo">
    <span>{{todo._id}}</span>
    <span>{{todo.name}}</span>
    <span>{{todo.description}}</span>
    <span>{{todo.done}}</span>
  </div>
</template>


<script>
export default {
  name: "Todo",
  props: {
    todo: Object
  }
};
</script>

<style>
.todo {
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 32px 16px;
}
</style>