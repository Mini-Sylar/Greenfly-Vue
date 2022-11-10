<template lang="">
    <div>
        <div class="footer-container">
            <div class="group-1">
                <div class="logo-important">
                    <img src="@/assets/images/logo.png" alt="">
                    <P>copyright &copy; {{year}} Greenfly all rights reserved</P>
                </div>
                <div class="location-important">
                    <div class="location">
                       <i class="fa-solid fa-location-dot"></i>
                        <p>Greenfly, 1234 Main Street, New York, NY 12345</p>
                    </div>
                    <div class="phone">
                       <i class="fa-solid fa-mobile"></i>
                        <p>Phone: 123-456-7890</p>
                    </div>
                    <div class="email">
                       <i class="fa-solid fa-envelope"></i>
                        <p>Email: example@gmail.com </p>
                        </div>
                </div>
                <div class="socials-important">
                    <div class="socials">
                       <i class="fa-brands fa-github"></i>
                        <p>Follow us on social media</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    data() {
        return {
            year: new Date().getFullYear()
        };
    },
}
</script>
<style src="@/assets/css/Footer.css" scoped>

</style>