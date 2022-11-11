<script>
import Banner from './Banner.vue';
import ComicsList from './ComicsList.vue';
export default {
    name: 'SiteMain',
    components: {
        ComicsList,
        Banner
    }
}
</script>

<template>

    <main id="site_main">

        <ComicsList></ComicsList>
        <Banner></Banner>





    </main>

</template>

<style lang="scss" scoped>
.icon {
    background-color: #0282F9;
}
</style>