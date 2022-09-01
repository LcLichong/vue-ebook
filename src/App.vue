<template>
    <div id="app">
        <span class="text">ABCDEFG</span>
        <router-view />
    </div>
</template>

<style>
html,
body {
    height: 100vh;
    margin: 0;
}
#app {
    height: 100%;
    font-family: Avenir, Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
}
.text {
    font-family: 'Days One';
    font-size: 20px;
    color: blue;
}
</style>
