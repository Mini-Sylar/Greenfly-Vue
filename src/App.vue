<template lang="">
  <div>
    <app-header></app-header>
    <section>
      <div class="is-a-container">
         <app-landing></app-landing>
      </div>
     
    </section>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Landing from "./components/Landing.vue";
export default {
  name: "app",
  components: {
    "app-header": Header,
    "app-landing": Landing,
  },
};
</script>
<style lang="" src="@/assets/css/Reset.css"></style>
