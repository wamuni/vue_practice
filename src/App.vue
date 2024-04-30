<template>
    <div class="box">
        <PersonComponent />
    </div>
</template>

<script lang="ts">
export default {
    name: 'App'
}
</script>

<script setup lang="ts">
import PersonComponent from './components/Person.vue'
</script>

<style>
.box {
    background-color: burlywood;
    border-radius: 10px;
    padding: 10px;
    box-shadow: 0 0 10px;
}
</style>
