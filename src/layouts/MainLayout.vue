<template>
  <q-layout view="lHh Lpr lFf">

    <q-page-container>
      <router-view />
    </q-page-container>
  </q-layout>
</template>

<script>


export default {
  name: 'MainLayout',
  components: {},
  data() {
    return {

    }
  }
}
</script>
<style scoped>
/* Custom styles for dark-themed layout */
.q-page-container {
  /* Imposta l'immagine come sfondo */
  background-image: url('https://i.pinimg.com/originals/aa/9c/4e/aa9c4eab78b237c0b8db56bcc37f91ad.jpg');
  /* background-image: url('/public/image/sfondoTeal.jpeg'); */
  /* Imposta la dimensione del background (puoi personalizzarla) */
  background-size: cover;
  background-repeat: no-repeat;
  background-attachment: fixed;

  /* background-color: #2596be; */
  color: #fff;
}
</style>
