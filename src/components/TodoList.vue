<template>
    <div>
        <TodoInputText v-model="newTodoText" @keydown.enter="addTodo"/>
        <TodoListItem :todos="todos" />
    </div>
</template>

<script>
import TodoInputText from '@/components/TodoInputText.vue';
import TodoListItem from '@/components/TodoListItem.vue';


export default {
    components:{
        TodoInputText,
        TodoListItem,

    },
    data(){
        return{
          todos: ["pomme", "poire", "chocolat"],
          newTodoText: "",
        };
        
    },
    methods: {
        addTodo(){
            const trimmedText = this.newTodoText.trim();
            if (trimmedText) {
            this.todos.push(trimmedText);
            this.newTodoText = "";
            }
        }
    }
};
</script>

<style>

</style>