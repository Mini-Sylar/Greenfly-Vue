<template lang="">
  <div>
    <div class="image-1">
        <img :src="images[0]" alt="">
    </div>
    <div class="image-2">
        <img :src="images[1]" alt="">
    </div>
    <div class="image-3">
        <img :src="images[2]" alt="">
    </div>
  </div>
</template>
<script>
export default {
    data() {
        return {
            images: ['./assets/images/subject-1', './assets/images/subject-2', './assets/images/subject-3']
        };
    },
}
</script>

<style src="@/assets/css/ImagesLanding.css">

</style>