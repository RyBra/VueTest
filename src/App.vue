<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png" />
    <HelloWorld msg="kek" />
    <FirstComponent first="ЙА РАБОАТЮ" />
    <TodoList v-bind:todos="todos" />
  </div>
</template>

<script>
import HelloWorld from "./components/HelloWorld.vue";
import FirstComponent from "./components/FirstComponent.vue";
import TodoList from "./components/todo/TodoList.vue";

export default {
  name: "app",
  data: function() {
    return {
      todos: [
        {
          _id: "5df3e5126019af23f856e051",
          name: "John",
          description: "Раз два три",
          done: true,
          __v: 0
        },
        {
          _id: "5df3e5136019af23f856e052",
          name: "John",
          description: "Раз два три",
          done: true,
          __v: 0
        },
        {
          _id: "5df3e5136019af23f856e053",
          name: "John",
          description: "Раз два три",
          done: true,
          __v: 0
        }
      ]
    };
  },
  components: {
    HelloWorld,
    FirstComponent,
    TodoList
  }
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
