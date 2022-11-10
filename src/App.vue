<template lang="">
  <div>
    <app-header></app-header>
    <section>
      <div class="is-a-container">
         <app-landing></app-landing>
      </div>
    </section>
    <section>
      <div class="is-a-container">
        <section>
                 <app-seewhy></app-seewhy>
        </section>
 
      </div>
    </section>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Landing from "./components/Landing.vue";
import SeeWhy from "./components/SeeWhy.vue";
export default {
  name: "app",
  components: {
    "app-header": Header,
    "app-landing": Landing,
    "app-seewhy": SeeWhy,
  },
};
</script>
<style lang="" src="@/assets/css/Reset.css"></style>
