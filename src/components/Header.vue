<template lang="">
    <div>
        <header>
            <nav class="nav-bar">
                <div class="logo">
                    <img src="@/assets/images/logo.png" alt="">
                </div>
                <div class="links">
                    <ul>
                        <li v-for="(link, index) in links" :key="index">
                            <a :href="link.url">{{ link.name }}</a>
                        </li>
                    </ul>
                </div>
                <div class="demo">
                    <div class="request">
                        <a href="#">Login</a>
                        <a href="#" class="getDemo">Get a Demo</a>
                    </div>
                </div>
            </nav>
        </header>
    </div>
</template>
<script>
export default {
    data() {
        return {
            links: [
                {
                    name: 'Solutions',
                    link: '#'
                },
                {
                    name: 'Platforms',
                    link: '#'
                },
                {
                    name: 'Customers',
                    link: '#'
                },
                {
                    name: 'Resources',
                    link: '#'
                },
                {
                    name: 'About',
                    link: '#'
                }
            ]
        }
    },
}
</script>
<style lang="" scoped src="@/assets/css/Header.css">


</style>