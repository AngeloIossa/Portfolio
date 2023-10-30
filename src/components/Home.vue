<template>
  <q-card flat bordered class="my-card absolute-right">
    <q-card-section class="q-pt-none text-center text">
      <span class="nameHome"><strong>Angelo Iossa</strong></span>
      <br>
      <span class="jobsHome">Junior Full Stack Developer</span>
    </q-card-section>
  </q-card>
</template>

<script>
export default {
  name: 'Home',
  data() {
    return {}
  }
}
</script>

<style>
.my-card {
  background-color: rgb(34, 34, 34);
  height: 100%;
  border-radius: 40px;
  width: 70%;
}

.text {
  top: 50%;
  transform: translateY(-50%);
}

.nameHome {
  color: white;
  font-size: 50px;
  font-family: poppins, Helvetica, sans-serif;
}

.jobsHome {
  color: rgb(187, 187, 187);
  font-size: 20px;
  font-family: poppins, Helvetica, sans-serif;
}
</style>
