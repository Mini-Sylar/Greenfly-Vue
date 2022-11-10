<template lang="">
  <div>
    <app-header></app-header>
    <main>
      <section>
        <div class="is-a-container">
          <app-landing></app-landing>
        </div>
      </section>
      <section>
        <div class="is-a-container">
          <app-seewhy></app-seewhy>
        </div>
      </section>
      <section>
        <div class="is-a-container">
           <app-sections v-bind:section_content='section_content.content_1'>
           </app-sections>
            <app-sections v-bind:section_content='section_content.content_2'>
           </app-sections>
        </div>
       
      </section>
    </main>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Landing from "./components/Landing.vue";
import SeeWhy from "./components/SeeWhy.vue";
import Sections from './components/Sections.vue';
export default {
  name: "Greenfly",
  data() {
    return {
      title: "Title",
      body: "Body",
      section_content: {
        content_1: {
          title: "Section 1",
          body: "Body section that is here",
        },
        content_2: {
          title: "Section 2",
          body: "Body section that is here",
        },
      },
    };
  },
  components: {
    "app-header": Header,
    "app-landing": Landing,
    "app-seewhy": SeeWhy,
    "app-sections": Sections,
  },
};
</script>
<style lang="" src="@/assets/css/Reset.css"></style>
