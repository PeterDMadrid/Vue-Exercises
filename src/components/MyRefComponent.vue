<script setup>
import { ref } from 'vue'

let userList = ref(['Mioch', 'John', 'Peter'])
let newUser = ref('')

const addUser = () => {
    const trimmed = newUser.value.trim()
    if (trimmed) {
        userList.value.push(trimmed)
        newUser.value = ''
    }
}

</script>

<template>
    <h1>UserList: {{ userList }}</h1>
    <input v-model="newUser" placeholder="Enter Name">
    <button @click="addUser">Add User</button>


</template>

<style></style>