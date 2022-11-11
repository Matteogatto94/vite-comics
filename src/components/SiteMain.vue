<script>
import Jumbotron from './Jumbotron.vue';
import Banner from './Banner.vue';
import ComicsList from './ComicsList.vue';
export default {
    name: 'SiteMain',
    components: {
        ComicsList,
        Banner,
        Jumbotron
    }
}
</script>

<template>

    <main id="site_main">
        <Jumbotron></Jumbotron>
        <ComicsList></ComicsList>
        <Banner></Banner>





    </main>

</template>

<style lang="scss" scoped>

</style>