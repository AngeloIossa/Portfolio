<template>
  <q-page>
    <q-page padding>
      <div class="row q-gutter-md centered-element max-width items-center no-margin" style="height: 100vh;">
        <div class="col-1 no-margin" style="width: 5%;"></div>
        <div class="col-8 q-pl-md q-ml-md" style="width: 85%;">
          <main-carousel ref="carousel"></main-carousel>
        </div>
        <div class="col-1 no-margin" style="width: 5%;">
          <control-carousel @showHome="showHome()" @showAboutMe="showAboutMe()"
          @showResume="showResume()" @showContact="showContact()"></control-carousel>
        </div>
      </div>
      <!-- <div class="col-1 no-margin" style="width: 10%;"></div> -->
    </q-page>
  </q-page>
</template>

<script>
import MainCarousel from 'src/components/MainCarousel.vue';
import ControlCarousel from 'src/components/ControlCarousel.vue';
export default {
  components: { MainCarousel, ControlCarousel },
  name: 'PageIndex',
  data() {
    return {

    }
  },
  methods: {
    showHome() {
      this.$refs.carousel.showHome();
    },
    showAboutMe() {
      this.$refs.carousel.showAboutMe();
    },
    showResume() {
      this.$refs.carousel.showResume();
    },
    showContact() {
      this.$refs.carousel.showContact();
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

.max-width {
  width: 100%;
}
</style>
