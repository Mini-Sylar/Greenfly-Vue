<template lang="">
  <div class="landing-page" id="landing">
    <div class="left-side gs_reveal gs_reveal_fromLeft">
      <h1 class="transform-heading">
        {{ heading }}
      </h1>
      <p class="catch-body">
        {{ catchBody }}
      </p>
      <button type="button" class="request-demo-button">Request a Demo</button>
    </div>
    <div class="right-side gs_reveal gs_reveal_fromRight">
        <app-image-piece></app-image-piece>
    </div>
  </div>
</template>

<script>
import ImagePiece from './interface/ImagePiece.vue';
export default {
  data() {
    return {
      heading: "Tranform Your Advocates into Brand Builders",
      catchBody:
        "Greenlfy is the leader in advocacy marketing. The Greenfly software platfom enables organizations of all sizes to harness the power of digital media to build awareness, increase loyalty, and drive revenue in our new digital-first world.",
    };
  },
  components: {
    "app-image-piece": ImagePiece,
  },
};
</script>
<style src="@/assets/css/Landing.css">

</style>
