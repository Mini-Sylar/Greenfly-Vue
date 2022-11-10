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
           <div class="reverse">
            <app-sections v-bind:section_content='section_content.content_2' style="display:flex;flex-direction:column-reverse">
           </app-sections>
           </div> 
        </div>
      </section>
       <!-- Grid Elements -->
       <section>
        <div class="is-a-container">
          <app-grid></app-grid>
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
import GridElements from './components/GridElements.vue';


export default {
  name: "Greenfly",
  data() {
    return {
      title: "Title",
      body: "Body",
      section_content: {
        content_1: {
          title: "Every Organization Has Advocates",
          body: "Greenfly enables you to activate and benefit from the social influence of athletes, talent,celebrities, employees,fans, brand ambassadors,sponsors,customers, partners, and more.",
          image: 'subject-2.png'
        },
        content_2: {
          title: "Turn Advocates Into Brand Builders",
          body: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nunc bibendum vestibulum tempus. Suspendisse eros nulla, congue a ante ut, bibendum consequat massa. Donec mattis aliquet nunc eu iaculis. Praesent eu mi sed tortor vestibulum mollis ut id urna. Aenean et tempus enim,",
          image: 'subject-3.png'
        },
      },
    };
  },
  components: {
    "app-header": Header,
    "app-landing": Landing,
    "app-seewhy": SeeWhy,
    "app-sections": Sections,
    "app-grid": GridElements,
  },
};
</script>
<style  src="@/assets/css/Reset.css">
 
</style>
