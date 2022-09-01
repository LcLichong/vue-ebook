<template>
    <div class="home">
        <span class="icon-bookmark"></span>
        <span class="text">ABCDEFG</span>
    </div>
</template>

<script>
import Epub from 'epubjs'
global.ePub = Epub
export default {
    name: 'Home',
    mounted() {},
}
</script>

<style scoped>
.home {
    height: 100%;
}
#read {
    height: 100%;
}
.icon-bookmark {
    font-size: 30px;
}
.text {
    font-family: 'Days One';
    font-size: 1rem;
    color: blue;
}
</style>
