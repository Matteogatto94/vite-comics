<script>
import Comic from './Comic.vue';
import Comics from '../data/comics.js';
export default {
    components: {
        Comic
    },
    data() {
        return {
            comic: Comics
        }
    }
}
</script>


<template>

    <div class="container">
        <span>CURRENT SERIES</span>
        <div class="comics row row-cols-md-6 g-4">
            <Comic v-for="comics in comic" :image="comics.thumb" :title="comics.series"></Comic>
        </div>
    </div>

</template>

<style lang="scss">

</style>