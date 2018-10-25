<template>
    <div id="app">
        <router-view></router-view>
        <FooterGuide v-show="$route.meta.showFooter"></FooterGuide>
    </div>
</template>

<script>
import FooterGuide from './components/FooterGuide/FooterGuide'
export default {
    components:{
        FooterGuide
    }
}
</script>

<style lang="stylus" rel="stylesheet/stylus">
    #app
        width 100%
        height 100%
        max-width 640px
        min-width 320px
        background-color #f5f5f5
        margin 0 auto
</style>