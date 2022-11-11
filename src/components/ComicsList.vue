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
        <span class="series">CURRENT SERIES</span>
        <div class="comics row row-cols-md-6 g-4">
            <Comic v-for="comics in comic" :image="comics.thumb" :title="comics.series"></Comic>
        </div>
        <div class="button_load d-flex justify-content-center py-3">
            <span class="loading">LOAD MORE</span>
        </div>

    </div>

</template>

<style lang="scss">
.container {

    .loading {
        background-color: #0282F9;
        padding: 0.75rem 5rem;
        font-weight: bold;
    }


    .series {
        background-color: #0282F9;
        padding: 1rem 3rem;
        font-weight: bold;

        &:hover {
            cursor: pointer;
        }
    }

    .comics {
        margin-top: 1rem;
    }


}
</style>