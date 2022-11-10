<template>
    <div>
        <div class="contact-container">
            <div class="left-side">
                <h2>Ready to start a conversation?</h2>
                <p>We are always willing and ready to transform advocates</p>
                <ul>
                    <li><i class="fa-solid fa-mobile"></i> +233 xx xx xxxx</li>
                    <li><i class="fa-solid fa-envelope"></i> example@example.com</li>
                </ul>
            </div>
            <div class="right-side">
                <div class="form-container">
                    <form action="#">
                        <div class="group">
                            <label for="name" class="name">Name</label>
                            <input type="text" name="name" id="name" required>
                            <span class="highlight"></span>
                            <span class="bar"></span>
                        </div>
                        <div class="group">
                            <label for="email">Email</label>
                            <input type="email" name="email" id="email" required>
                            <span class="highlight"></span>
                            <span class="bar"></span>

                        </div>
                        <div class="group">
                            <label for="subject">Subject</label>
                            <input type="text" name="subject" id="subject" required>
                            <span class="highlight"></span>
                            <span class="bar"></span>

                        </div>
                        <div class="group">
                            <label for="message">Message</label>
                            <textarea name="message" id="message" cols="30" rows="10" required></textarea>
                            <span class="highlight"></span>
                            <span class="bar"></span>
                        </div>
                        <button type="submit">Send</button>
                    </form>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    data() {
        return {

        };
    },

}
</script>
<style scoped src="@/assets/css/Contact.css" >
    
</style>