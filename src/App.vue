<template>
  <div id="app" class="container">
    <h1 class="title is-1">boujour a vous</h1>
    <TodoList />
  </div>
</template>

<script>
import TodoList from '@/components/TodoList.vue';



export default {
  name: "app",
  components: {
    TodoList,
    
  }
};
</script>

<style lang="scss">
.container {
  margin: 100px 60px 0 100px};
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: red;
  margin-top: 60px;
}
</style>
