<template>
  <div id="app" class="container">
    <h1 class="title is-1">VUE TODO LIST</h1>
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
body{
  text-align: center;
}
.container {
  margin: 100px 60px 0 100px};
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color:red;
  margin-top: 60px;
  font-size: 3rem;
  font-weight: bold;
}
.title{
  color: cyan ;
  font-weight: bold;
  font-size: 4rem;
}
.input{
  border: 10px inset black;
  box-shadow: 3px 3px 3px yellow, 0 0 3em red, 0 0 3em red;
  margin-bottom: 2rem;
  text-align: center;
  color: whitesmoke;
  font-weight: bold;
  position: relative;
}  
  ::placeholder
  {
    font-size: 1.5rem;
    font-weight: bold;
    text-shadow: 2px 2px whitesmoke;
  }
</style>
