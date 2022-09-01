<template>
    <div id="app">
        <router-view />
    </div>
</template>

<script>
export default {}
document.addEventListener('DOMContentLoaded', () => {
    const html = document.querySelector('html')
    let fontSize = window.innerWidth / 10
    fontSize = fontSize > 50 ? 50 : fontSize
    html.style.fontSize = fontSize + 'px'
})
</script>

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
</style>
