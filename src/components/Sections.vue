<template lang="">
  <div>
    <div>
        <div class="left-side">
           <h2>{{section_content.title}}</h2>
        </div>    
        <div class="right-side">
            Image Here
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
<style lang=""></style>
