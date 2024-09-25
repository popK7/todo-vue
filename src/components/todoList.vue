<template>
    <!-- nav -->
    <div class="nav-bar">
        <h3>Taches</h3>
        <div class="mt-10">
            <button>Ajouter</button>
        </div>
    </div>
    <!-- search -->
    <div class="search">
        <search-task />
    </div>

    <!-- Tasks -->
    <div class="tasks">
        <todo v-for="task in tasks" :key="task.id" :todo="task" />
    </div>
</template>
<script setup>
import { reactive } from "vue";
import searchTask from './SearchTask.vue'
import todo from './TodoSimple.vue' 
 let tasks = reactive([
    {id: 1, name: "faire malessive", done:false},
    {id: 2, name: "Cuisiner le chips", done:false},
    {id: 3, name: "Aller à la maison", done:false},
    {id: 4, name: "Loca locca", done:true}
 ]);
   
</script>

<style>
    .nav-bar{
        width: 50%;
        display: flex;
        justify-content: space-between;
        margin: auto 25%;
    }

    .mt-10 {
        margin-top: 2.5%;
    }
</style>