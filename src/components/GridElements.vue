<template lang="">
  <div class="grid-container">
    <h2 class="main-section-title gs_reveal">Lorem Ipusm</h2>
      <div class="grid-elements">
        <div class="gs_reveal" v-for="(item, index) in content.icons" :key="index">
          <div class="grid-item">
            <h4><i :class="item"></i></h4>
            <h5>{{ content.body[index] }}</h5>
          </div>
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
    column-gap: 1rem;
    /* width: 100%;
    margin: 0 auto; */
}

h2 {
    text-align: center;
    margin-bottom: 2rem;
    font-size: clamp(1.7rem, 2.5vw, 2.5rem);
}

h4,
h5 {
    text-align: center;
    margin: 0 auto;
    /* width: 30ch; */
}

h5 {
    width: 25ch;
    font-size: clamp(.8rem, 1vw, 1.5rem);
}

h4 {
    font-size: 14px;
    margin-block: .5rem;
}

h4>* {
    color: var(--main-accent-color);
    font-size: 2.5rem;
}

.grid-container {
    padding: 3rem;
}

@media screen and (max-width: 426px) {
    .grid-elements {
        display: grid;
        grid-template-columns: repeat(2, 1fr);
        grid-template-rows: repeat(3, 1fr);
        grid-template-areas:
            "a b"
            "c d"
            "e f";
        place-items: center;
        height: 100%;
        column-gap: 2rem;
        /* width: 100%;
    margin: 0 auto; */
    }

    h4>* {
        color: var(--main-accent-color);
        font-size: 2.2rem;
    }

    h5 {
        width: 20ch;
        font-size: clamp(.7rem, .2vw, 1.5rem);
    }
}
</style>
