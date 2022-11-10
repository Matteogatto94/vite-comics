<script>
import SiteHeader from './components/SiteHeader.vue'
import SiteMain from './components/SiteMain.vue'
import SiteFooter from './components/SiteFooter.vue'
export default {
    name: 'App',
    components: {
        SiteHeader,
        SiteMain,
        SiteFooter
    }
}
</script>

<template>

    <site-header></site-header>
    <!-- /#site_header -->

    <site-main></site-main>
    <!-- /#site_main -->

    <site-footer></site-footer>
    <!-- /#site_footer -->

</template>

<style lang="scss">

</style>
