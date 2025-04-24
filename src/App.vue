<template>
    <div class="app">
        <h1>Hello World</h1>
        <Person />
    </div>
</template>

<script lang="ts">
import Person from './components/Person.vue'
export default {
    name: 'App',
    components: {
        Person
    }
}
</script>

<style scoped>
.app {
    background-color: #f0f0f0;
    padding: 20px;
    border-radius: 10px;
}
</style>
