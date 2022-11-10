<template lang="">
  <div>
    <app-header></app-header>
     <ui-blob></ui-blob>
    <main>
       <ui-wave></ui-wave>
      <section>
        <div class="is-a-container is-landing">
          <app-landing ></app-landing>
        </div>
      </section>
      <section class="has-color push-up">
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
      </section >
       <!-- Grid Elements -->
       <section class="has-color">
        <div class="is-a-container">
          <app-grid></app-grid>
        </div>
       </section>
       <!-- Contact Section -->
      <section>
        <div class="is-a-container">
          <app-contact></app-contact>
        </div>
      </section>
    </main>
    <!-- Footer -->
    <footer class="is-a-footer">
      <app-footer></app-footer>
    </footer>
  </div>
</template>

<script>
import Header from "./components/Header.vue";
import Landing from "./components/Landing.vue";
import SeeWhy from "./components/SeeWhy.vue";
import Sections from './components/Sections.vue';
import GridElements from './components/GridElements.vue';
import Contact from './components/Contact.vue';
import Footer from './components/Footer.vue';
import Wave from './components/interface/Wave.vue';
import Blob from './components/interface/Blob.vue';

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
    "app-contact": Contact,
    "app-footer": Footer,
    "ui-wave": Wave,
    "ui-blob": Blob,
  },
};
</script>
<style  src="@/assets/css/Reset.css">

</style>
