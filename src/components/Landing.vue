<template lang="">
  <div class="landing-page">
    <div class="left-side">
      <h1 class="transform-heading">
        {{ heading }}
      </h1>
      <p class="catch-body">
        {{ catchBody }}
      </p>
      <button type="button" class="request-demo-button">Request a Demo</button>
    </div>
    <div class="right-side"></div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      heading: "Tranform Your Advocates into Brand Builders",
      catchBody:
        "Greenlfy is the leader in advocacy marketing. The Greenfly software platfom enables organizations of all sizes to harness the power of digital media to build awareness, increase loyalty, and drive revenue in our new digital-first world.",
    };
  },
};
</script>
<style lang="" src="@/assets/css/Landing.css">
  @import './assets/css/Reset.css';
</style>
