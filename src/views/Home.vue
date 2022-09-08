<template>
    <div class="home">
        <span class="icon-bookmark"></span>
        <span class="text">ABCDEFG</span>
    </div>
</template>

<script>
import Epub from 'epubjs'
import { mapGetters } from 'vuex'
global.ePub = Epub

const getters = {
    a: () => 1,
    b: () => 2,
    c: () => 3,
}
function fn(keys) {
    const data = {}
    keys.forEach((key) => {
        // eslint-disable-next-line no-prototype-builtins
        if (getters.hasOwnProperty(key)) {
            data[key] = getters[key]
        }
    })
    return data
}
export default {
    name: 'Home',
    computed: {
        ...mapGetters(['test']),
        ...fn(['a', 'b', 'c']),
    },
    mounted() {
        // console.log(this.test)
        // this.$store.dispatch('setTest', 9).then(() => {
        //     console.log(this.test)
        // })
        console.log(this.a)
        console.log(this.b)
        console.log(this.c)
    },
}
</script>

<style lang="scss" scoped>
@import '../assets/styles/global.scss';
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
    font-size: px2rem(20);
    color: blue;
}
</style>
