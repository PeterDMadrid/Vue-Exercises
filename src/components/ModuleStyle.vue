<template>
    <!-- <h1 :class="$style['m-class']">Using Module Css with $ syntax kebab case</h1> -->
    <h1 :class="myClass.anotherClass">Using Module CSS using $ camel case</h1>
</template>

<style module="myClass">
.m-class {
    background: firebrick;
    color: white;
}

.anotherClass {
    background: seagreen;
    color: white;
}
</style>