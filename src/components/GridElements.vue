<template lang="">
  <div class="grid-elements">
    <div class="" v-for="(item, index) in content.icons" :key="index">
      <div class="grid-item">
        <h4><i :class="item"></i></h4>
        <h5>{{ content.body[index] }}</h5>
      </div>
    </div>
  </div>
</template>
<script>
export default {
    data() {
        return {
            content: {
                icons: [
                    "fas fa-monitor-heart-rate",
                    "fa-solid fa-hands-bubbles",
                    "fa-solid fa-heart-half-stroke",
                    "fas fa-calendar-alt",
                    "fa-solid fa-arrow-trend-up",
                    "fas fa-popcorn",
                ],

                body: [
                    "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin felis eros, condimentum nec eros ut, commodo imperdiet sem.",
                    "Sed id mi posuere, condimentum augue at, finibus ligula. Quisque fermentum ligula quis est rhoncus, ut pharetra tortor dapibus.",
                    "Sed id mi posuere, condimentum augue at, finibus ligula. Quisque fermentum ligula quis est rhoncus, ut pharetra tortor dapibus.",
                    " Phasellus vitae suscipit ex. Ut porttitor malesuada tortor, non efficitur nunc pharetra at. Nulla rutrum orci sed scelerisque tristique.",
                    "Sed ultrices mi ut lorem sollicitudin, et iaculis eros gravida. Duis fringilla quam ex, ac molestie purus dapibus maximus.",
                    "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Proin felis eros, condimentum nec eros ut, commodo imperdiet sem. ",
                ],
            },
        };
    },
};
</script>
<style scoped>
.grid-elements {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: repeat(2, 1fr);
    grid-auto-columns: 1fr;
    grid-auto-rows: 1fr;
    grid-template-areas:
        "a b c"
        "d e f";
    place-items: center;
    height: 50vh;
    width: 100%;

}

h4,
h5 {
    text-align: center;
    margin: 0 auto;
    width: 30ch;
}

h4 {
    font-size: 18px;
    margin-block: .5rem;
}

h4>* {
    color: #41b883;
    font-size: 2rem;
}
</style>
