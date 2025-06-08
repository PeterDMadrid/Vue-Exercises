<script setup>
import { reactive } from 'vue';
let initialState = reactive({
    val: {
        count: 0,
    },
    user: ['John', 'Dave']
})

function changeUser() {
    initialState.user[0] = 'Micheal'
    initialState.user[1] = 'Philip'
}


</script>

<template>
    <h1>Current Count: {{ initialState.val.count }}</h1>
    <h2>Users: {{ initialState.user }}</h2>
    <button @click="initialState.val.count += 10">Add 10</button>
    <button @click="changeUser">Change user</button>
    <button @click="initialState.user.push('asdasd')">Add one more</button>
</template>
