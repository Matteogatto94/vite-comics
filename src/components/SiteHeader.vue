<script>

export default {
    name: 'SiteHeader',
    data() {
        return {
            menu: [
                {
                    text: 'Characters',
                    href: '#'
                },
                {
                    text: 'Comics',
                    href: '#'
                },
                {
                    text: 'Movies',
                    href: '#'
                },
                {
                    text: 'TV',
                    href: '#'
                },
                {
                    text: 'Games',
                    href: '#'
                },
                {
                    text: 'Collectibles',
                    href: '#'
                },
                {
                    text: 'Videos',
                    href: '#'
                },
                {
                    text: 'Fans',
                    href: '#'
                },
                {
                    text: 'News',
                    href: '#'
                },
                {
                    text: 'Shop',
                    href: '#'
                }
            ]
        }
    }
}
</script>

<template>

    <header id="site_header">
        <div class="container">
            <div class="navbar">
                <div class="logo">
                    <img src="../assets/img/dc-logo.png" alt="">
                </div>

                <div class="navbar_right">
                    <a :href="item.href" v-for="item in menu">
                        {{ item.text }}
                    </a>
                </div>
            </div>

        </div>

    </header>

</template>

<style lang="scss" scoped>

</style>