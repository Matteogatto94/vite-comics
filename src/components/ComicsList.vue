<script>
import Comics from '../data/comics.js';
export default {
    components: {

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
        <div class="row">
            <div class="col" v-for="comics in comic">
                <img :src="comics.thumb" alt="Action Comics">
                <p>{{ comics.series }}</p>
            </div>
        </div>
    </div>

</template>

<style lang="scss">

</style>