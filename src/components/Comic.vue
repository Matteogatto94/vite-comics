<script>
export default {
    name: 'Comic',
    props: {
        image: String,
        title: String
    }
}
</script>

<template>

    <div class="col">
        <div class="comics">
            <img :src="image" :alt="title">
            <h4>{{ title }}</h4>
        </div>
    </div>

</template>

<style lang="scss">
.comics {

    h4 {
        padding: 1rem;
        text-align: center;
        font-size: 20px;
    }
}
</style>