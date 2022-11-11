<template lang="">
    <div>
        <aside class="nav-mobile">
        <a href="#">Solutions</a>
        <a href="#">Platform</a>
        <a href="#">Customers</a>
        <a href="#">Resource</a>
        <a href="#">About</a>
        </aside>
         <aside class="first"></aside>
    </div>
</template>
<script>

export default {
    data() {
        return {
        }
    },

}
</script>
<style scoped>
.nav-mobile {
    width: 0;
    height: 100vmax;
    background-color: #333;
    position: absolute;
    display: flex;
    justify-content: center;
    align-items: center;
    z-index: 3;
    flex-direction: column;
    gap: 2rem;
    right: 0;
    visibility: hidden;
    transition: all 1s ease;
    overflow: hidden;
}

.first {
    display: block;
    content: "";
    position: absolute;
    width: 10%;
    height: 100vmax;
    background-color: var(--main-accent-color);
    z-index: 1;
    right: 0;
    visibility: hidden;
    transition: all 0.5s ease;
}

.nav-mobile>a {
    color: #fff;
    font-size: 25px;
    font-weight: 900;
    transition: all 1s ease-in;
    opacity: 1;
}

.show-nav {
    width: 100%;
    visibility: visible;
}
</style>