<template>
    <header>
        <h1>{{title}}</h1>
        <Button @toggle-add-task="$emit('toggle-add-task')" :text="showAddTask ? 'Close' : 'Add Task'" :color="showAddTask ? 'red' : 'green'"  />
    </header>
</template>

<script>
 import Button from './button'

    export default{
        name: 'Header',
        props: {
            title: String,
            showAddTask: Boolean,
        },
        components: {
            Button
        }
    }
</script>

<style scooped>
    header{
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin-bottom: 20px;
    }
</style>