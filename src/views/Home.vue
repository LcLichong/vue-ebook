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

<style lang="scss" scoped>
.home {
    height: 100%;
}
#read {
    height: 100%;
}
.icon-bookmark {
    font-size: 30px;
}
@import '../assets/styles/global.scss';
.text {
    font-size: px2rem(20);
    color: blue;
}
</style>
