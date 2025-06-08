<script setup>
import { ref } from 'vue'

let isLoggedIn = ref(false)

let username = ref('Peter')
const login = () => {
    isLoggedIn.value = !isLoggedIn.value
}

</script>

<template>
    <div>
        <button v-if="isLoggedIn" @click="login">Logout</button>
        <button v-else @click="login">Login</button>
        <p v-if="isLoggedIn">Welcome, {{ username }}</p>
        <p v-if="!isLoggedIn">Please Login</p>
    </div>
</template>
