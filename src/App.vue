<template lang="">
  <div>
    <app-header v-if="!isMobile()"></app-header>
    <ui-mobile-header v-else></ui-mobile-header>
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
            <app-sections v-bind:section_content='section_content.content_2'>
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
import MobileHeaderVue from "./components/mobile/MobileHeader.vue";
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
    "ui-mobile-header": MobileHeaderVue
  },
  methods: {
    isMobile: function () {
      var check = false;
      (function (a) { if (/(android|bb\d+|meego).+mobile|avantgo|bada\/|blackberry|blazer|compal|elaine|fennec|hiptop|iemobile|ip(hone|od)|iris|kindle|lge |maemo|midp|mmp|mobile.+firefox|netfront|opera m(ob|in)i|palm( os)?|phone|p(ixi|re)\/|plucker|pocket|psp|series(4|6)0|symbian|treo|up\.(browser|link)|vodafone|wap|windows ce|xda|xiino/i.test(a) || /1207|6310|6590|3gso|4thp|50[1-6]i|770s|802s|a wa|abac|ac(er|oo|s\-)|ai(ko|rn)|al(av|ca|co)|amoi|an(ex|ny|yw)|aptu|ar(ch|go)|as(te|us)|attw|au(di|\-m|r |s )|avan|be(ck|ll|nq)|bi(lb|rd)|bl(ac|az)|br(e|v)w|bumb|bw\-(n|u)|c55\/|capi|ccwa|cdm\-|cell|chtm|cldc|cmd\-|co(mp|nd)|craw|da(it|ll|ng)|dbte|dc\-s|devi|dica|dmob|do(c|p)o|ds(12|\-d)|el(49|ai)|em(l2|ul)|er(ic|k0)|esl8|ez([4-7]0|os|wa|ze)|fetc|fly(\-|_)|g1 u|g560|gene|gf\-5|g\-mo|go(\.w|od)|gr(ad|un)|haie|hcit|hd\-(m|p|t)|hei\-|hi(pt|ta)|hp( i|ip)|hs\-c|ht(c(\-| |_|a|g|p|s|t)|tp)|hu(aw|tc)|i\-(20|go|ma)|i230|iac( |\-|\/)|ibro|idea|ig01|ikom|im1k|inno|ipaq|iris|ja(t|v)a|jbro|jemu|jigs|kddi|keji|kgt( |\/)|klon|kpt |kwc\-|kyo(c|k)|le(no|xi)|lg( g|\/(k|l|u)|50|54|\-[a-w])|libw|lynx|m1\-w|m3ga|m50\/|ma(te|ui|xo)|mc(01|21|ca)|m\-cr|me(rc|ri)|mi(o8|oa|ts)|mmef|mo(01|02|bi|de|do|t(\-| |o|v)|zz)|mt(50|p1|v )|mwbp|mywa|n10[0-2]|n20[2-3]|n30(0|2)|n50(0|2|5)|n7(0(0|1)|10)|ne((c|m)\-|on|tf|wf|wg|wt)|nok(6|i)|nzph|o2im|op(ti|wv)|oran|owg1|p800|pan(a|d|t)|pdxg|pg(13|\-([1-8]|c))|phil|pire|pl(ay|uc)|pn\-2|po(ck|rt|se)|prox|psio|pt\-g|qa\-a|qc(07|12|21|32|60|\-[2-7]|i\-)|qtek|r380|r600|raks|rim9|ro(ve|zo)|s55\/|sa(ge|ma|mm|ms|ny|va)|sc(01|h\-|oo|p\-)|sdk\/|se(c(\-|0|1)|47|mc|nd|ri)|sgh\-|shar|sie(\-|m)|sk\-0|sl(45|id)|sm(al|ar|b3|it|t5)|so(ft|ny)|sp(01|h\-|v\-|v )|sy(01|mb)|t2(18|50)|t6(00|10|18)|ta(gt|lk)|tcl\-|tdg\-|tel(i|m)|tim\-|t\-mo|to(pl|sh)|ts(70|m\-|m3|m5)|tx\-9|up(\.b|g1|si)|utst|v400|v750|veri|vi(rg|te)|vk(40|5[0-3]|\-v)|vm40|voda|vulc|vx(52|53|60|61|70|80|81|83|85|98)|w3c(\-| )|webc|whit|wi(g |nc|nw)|wmlb|wonu|x700|yas\-|your|zeto|zte\-/i.test(a.substr(0, 4))) check = true; })(navigator.userAgent || navigator.vendor || window.opera);
      return check;
    }
  },
};
</script>
<style  src="@/assets/css/Reset.css">

</style>
