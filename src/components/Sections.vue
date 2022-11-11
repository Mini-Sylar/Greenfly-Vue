<template lang="">
  <div>
    <div class="content-section">
        <div class="left-side gs_reveal gs_reveal_fromLeft" >
           <h2>{{section_content.title}}</h2>
           <p>{{section_content.body}}</p>
        </div>    
        <div class="right-side gs_reveal gs_reveal_fromRight">
            <img :src="image"  alt="Image Here">
        </div>
    </div>
  </div>
</template>
<script>
export default {
    data() {
        return {
        }
    },
    props: {
        section_content: {
            type: Object,
            // required: true
        }
    },
    computed: {
        image: function () {
            return new URL(`/src/assets/images/${this.section_content.image}`, import.meta.url)
        }
    }
};
</script>
<style scoped>
.content-section {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    height: 50vh;
    margin-block: 2rem;
    padding: 1.5rem;
    gap: 2rem;
}


.left-side,
.right-side {
    width: 100%;
    height: 90%;
    display: flex;
    flex-direction: column;
    gap: 1rem;
    border-radius: 20px;
    justify-content: center;
}

p {
    width: 50ch;
    font-size: clamp(.7rem, 1.5vw, 1.2rem);
}

h2 {
    font-size: clamp(1.7rem, 2.5vw, 2.5rem);
}

img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    border-radius: 20px;

}

@media screen and (max-width: 427px) {
    .content-section {
        flex-direction: column;
        height: 100%;

    }

    p {
        width: 35ch;
        font-size: clamp(1rem, 1.5vw, 2rem);
    }



}
</style>
