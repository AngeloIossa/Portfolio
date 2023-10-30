<template>
  <q-carousel class="bg-gray rounded-carousel carouselHeight" v-model="slide" scrollable>
    <!-- HOME -->
    <q-carousel-slide name="home" class="column no-wrap flex-center">
      <main-information></main-information>
      <home></home>
    </q-carousel-slide>
    <!-- ABOUT ME -->
    <q-carousel-slide name="about_me" class="column flex-center">
      <main-information></main-information>
      <about-me></about-me>
    </q-carousel-slide>
    <!-- RESUME -->
    <q-carousel-slide name="resume" class="column flex-center">
      <main-information></main-information>
      <resume></resume>
    </q-carousel-slide>
    <!-- CONTACT -->
    <q-carousel-slide name="contact" class="column flex-center">
      <main-information></main-information>
      <contact></contact>
    </q-carousel-slide>
  </q-carousel>
</template>

<script>
import { ref } from 'vue';
import Home from './Home.vue';
import MainInformation from './MainInformation.vue';
import AboutMe from './AboutMe.vue';
import Resume from './Resume.vue';
import Contact from './Contact.vue';

const HOME = 'home';
const ABOUT_ME = 'about_me';
const RESUME = 'resume';
const CONTACT = 'contact';

export default {
  components: { Home, MainInformation, AboutMe, Resume, Contact },
  // name: 'ComponentName',
  data() {
    return {
      slide: ref('home'),
      lorem: 'My carousel',
    }
  },
  methods: {
    showHome() {
      console.log('Evento arrivato');
      this.slide = HOME;
    },
    showAboutMe() {
      this.slide = ABOUT_ME;
    },
    showResume() {
      this.slide = RESUME;
    },
    showContact() {
      this.slide = CONTACT;
    },
  }
}
</script>
<style>
.centered-element {
  /* margin: 0; */
  position: absolute;
  top: 50%;
  transform: translateY(-50%);
}

.carouselHeight {
  height: 85vh;
}

.bg-gray {
  background-color: rgb(68,68,68);
  /* Change this to your desired shade of gray */
}

.rounded-carousel {
  border-radius: 40px;
  /* Imposta il valore del bordo arrotondato desiderato */
}
</style>
