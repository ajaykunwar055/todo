<template>
    <div>
        <h1>Todo App</h1>
        <input type="text" v-model="todo"/>  
        <button @click="add">  Add</button>
        <br>
     
     <ol>
            <li v-for="todo in todos" :key="todo.list">
        {{todo}} 
            <button @click="removeTodo(index)">Delete</button>

        <br>
        </li>
        </ol>
    </div>
</template>

<script>
export default {
       data(){ 
           return {
           todo:'',
           todos:['Learn Vue']
        }
       },
       methods: {
           add(){
       this.todos.push(this.todo);
       this.todo = ''
       },
         removeTodo(index) {
         this.todos.splice(index, 1)
                },
       }
}
</script>

<style>
  
</style>