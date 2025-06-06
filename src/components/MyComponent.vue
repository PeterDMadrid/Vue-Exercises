<script setup>
const mymessage = "Yellow World"
const myNumber = 100
function add(x, y) {
    return x + y
}
</script>

<template>
    <h1>{{ mymessage }}</h1>
    <h2>{{ myNumber }}</h2>
    <h2>2 + 2 = {{ 2 + 2 }}</h2>
    <h1>Add Two Numbers: {{ add(2, 5) }}</h1>
</template>
