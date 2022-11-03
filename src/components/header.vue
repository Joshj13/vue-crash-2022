<template>
    <header>
        <h1>Task Tracker</h1>
        <Button text="Add Task" color ="green" />
    </header>
</template>

<script>
 import Button from './button'

    export default{
        name: 'Header',
        props: {
            title: String,
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