<template>
  <q-card flat class="information-card absolute-left">

    <q-card-section class="q-pt-none text-center" style="margin-top: 20%;">
      <q-avatar size="200px" font-size="52px" color="teal" text-color="white" icon="person" class="my-avatar shadow-14"/>
    </q-card-section>

    <q-card-section class="text-center">
      <span class="nameInformation"><strong>Angelo Iossa</strong></span><br>
      <span class="jobsInformation">Junior Full Stack Developer</span>
    </q-card-section>
    <q-card-section class="text-center">
      <q-btn round flat class="q-mr-sm">
        <i class="fa-brands fa-instagram fa-2xl"></i>
      </q-btn>
      <q-btn round flat class="q-mr-sm">
        <i class="fa-brands fa-github fa-2xl"></i>
      </q-btn>
      <q-btn round flat >
        <i class="fa-brands fa-linkedin-in fa-2xl"></i>
      </q-btn>
    </q-card-section>
    <q-card-section class="text-center" style="margin-top: 10%;">
      <q-btn rounded outline label="Download CV" size="md" class="q-px-md"></q-btn>
    </q-card-section>
  </q-card>
</template>

<script>
export default {
  // name: 'ComponentName',
  data () {
    return {}
  }
}
</script>
<style>
.information-card {
  background-color: rgb(68,68,68);
  height: 100%;
  border-radius: 40px;
  width: 30%;

}
.nameInformation {
  color: white;
  font-size: 36px;
  font-family: poppins,Helvetica,sans-serif;
}
.jobsInformation {
  color: rgb(187, 187, 187);
  font-size: 18px;
  font-family: poppins,Helvetica,sans-serif;
}
</style>
