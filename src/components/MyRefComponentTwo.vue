<script setup>
import { ref, reactive } from 'vue'
let userInfo = reactive({
    name: 'Peter',
    age: 23,
    location: ['QC', 'PH'],
    isMarried: false
})
</script>
<template>
    <h1>Name: {{ userInfo.name }}</h1>
    <h1>Age: {{ userInfo.age }}</h1>
    <h1>Location: {{ userInfo.location.join(', ') }}</h1>
    <h1>isMarried: {{ userInfo.isMarried }}</h1>
</template>
<style scope></style>