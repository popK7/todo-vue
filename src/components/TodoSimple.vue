<template>
    <div class="todo">
        <p>{{todo.name}}</p>
        <p>
            <button>Done</button>
            <button>Remove</button>
        </p>
    </div>
</template>

<script setup> 
     const props = defineProps({
        todo:{ 
            type: Object,
            default: () => {}
        }
    });
</script>

<style>
    .todo {
        display: flex;
        justify-content: space-between;
        margin: auto 25%;
    }
</style>