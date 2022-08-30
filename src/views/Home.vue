<template>
    <div class="home">
        <div id="read"></div>
    </div>
</template>

<script>
import Epub from 'epubjs'
global.ePub = Epub
export default {
    name: 'Home',
    mounted() {
        this.book = new Epub('/1.epub')
        console.log(this.book)
        this.book
            .renderTo('read', {
                width: window.innerWidth,
                height: window.innerHeight,
            })
            .display()
    },
}
</script>

<style lang="less">
.home {
    height: 100%;
    #read {
        height: 100%;
    }
}
</style>
