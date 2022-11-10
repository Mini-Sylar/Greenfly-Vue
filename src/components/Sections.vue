<template lang="">
  <div>
    <div class="content-section">
        <div class="left-side">
           <h2>{{section_content.title}}</h2>
           <p>{{section_content.body}}</p>
        </div>    
        <div class="right-side">
            <img src="@/assets/images/subject-2.png"  alt="Image Here">
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
    methods: {
        changeTitle: function (params) {

        }
    },
    props: {
        section_content: {
            type: Object,
            // required: true
        }
    },
    // created: function (whichcontent) {
    //     this.title = this.section_content.whichcontent.title;
    //     this.body = this.section_content.whichcontent.body;
    // },
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
    /* align-items: center; */
}

p {
    width: 50ch;
}

h2 {
    font-size: clamp(1.5rem, 3vw, 4rem);
}

img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    /* padding: 1rem; */
    border-radius: 20px;

}
</style>
