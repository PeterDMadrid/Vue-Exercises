<script setup>
// const myChannel = "https://vuejs.org/guide/introduction.html"
// const image = "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTc9APxkj0xClmrU3PpMZglHQkx446nQPG6lA&s"
// const altText = "dynamic alt"
// const imageWidth = 400
// const imageHeight = 400
const imageInfo = {
    src: 'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTc9APxkj0xClmrU3PpMZglHQkx446nQPG6lA&s',
    alt: 'random text',
    width: 500,
    height: 500
}
</script>

<template>
    <a :href="myChannel">Vue guide</a>
    <img :="imageInfo">
</template>
