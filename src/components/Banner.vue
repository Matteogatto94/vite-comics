<script>
export default {
    name: 'Banner',
    data() {
        return {
            items: [
                {
                    icon: 'buy-comics-digital-comics.png',
                    text: 'Digital Comics'
                },
                {
                    icon: 'buy-comics-merchandise.png',
                    text: 'DC Merchandise'
                },
                {
                    icon: 'buy-comics-shop-locator.png',
                    text: 'Subscription'
                },
                {
                    icon: 'buy-comics-subscriptions.png',
                    text: 'Comic Shop Locator'
                },
                {
                    icon: 'buy-dc-power-visa.svg',
                    text: 'DC Power Visa'
                }
            ]
        }
    },
    methods: {
        getImageUrl(name) {
            return new URL(`../assets/img/${name}`, import.meta.url).href
        }
    }
}


</script>

<template>

    <div class="banner">
        <div class="container d-flex justify-content-evenly align-items-center">
            <div class="item" v-for="item in items">
                <img :src="getImageUrl(item.icon)" alt="">
                <span>{{ item.text }}</span>
            </div>
        </div>
    </div>


</template>

<style lang="scss">
.banner {
    background-color: #0282F9;
    padding: 3rem;

    span {
        padding: 1rem;
        font-size: 1rem;
    }

    img {
        width: 50px;
    }
}
</style>