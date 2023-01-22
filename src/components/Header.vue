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
                            <a :href="link.to">{{ link.name }}</a>
                        </li>
                    </ul>
                </div>
                <div class="demo">
                    <div class="request">
                        <a href="#">Login</a>
                        <a href="#" class="get-demo">Get a Demo</a>
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
                    link: '#',
                    to:"#landing"
                },
                {
                    name: 'Platforms',
                    link: '#',
                    to:"#seewhy"
                },
                {
                    name: 'Customers',
                    link: '#',
                    to: "#content-section-main"
                },
                {
                    name: 'Resources',
                    link: '#',
                    to:'#resources-used'
                },
                {
                    name: 'Contact',
                    link: '#',
                    to:'#contact'
                }
            ]
        }
    },
}
</script>
<style scoped src="@/assets/css/Header.css">


</style>