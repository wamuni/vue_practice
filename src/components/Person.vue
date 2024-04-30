<template>
    <div class="person">
        <h2>Name: {{ name }}</h2>
        <h4>Age: {{ age }}</h4>
        <h4>Address: {{ address }}</h4>
        <button @click="changeName">Change Name</button>
        <button @click="changeAge">Change Age</button>
    </div>
</template>

<script lang="ts">
import { ref } from 'vue'
export default {
    name: 'PersonComponent'
}
</script>

<script setup lang="ts">
let name = ref('Eddie')
let age = ref(18)
let address = 'Ardpatrick Louth Village'

function changeName() {
    name.value = 'Eddiddie'
}

function changeAge() {
    age.value += 1
}
</script>

<style scoped>
.person {
    box-shadow: 0 0 10px;
    border-radius: 10px;
    background-color: cadetblue;
    padding: 10px;
}

button {
    margin: 10px;
    padding: 10px;
    border-radius: 5px;
    background-color: chocolate;
}
</style>
