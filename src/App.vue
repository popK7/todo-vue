<template>
  <todo-list />
</template>

<script>
import todoList from './components/todoList.vue'
export default {
  name: 'App',
  components: {
    todoList
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}

.id{
  display: none;
  justify-content: center;
}
</style>
