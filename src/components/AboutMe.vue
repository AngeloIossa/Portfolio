<template>
  <q-card flat bordered class="my-card absolute-right q-pa-xl">
    <q-card-section>
      <span class="about-me"><strong>About <span class="personalInformationLabel">Me</span></strong></span>
    </q-card-section>

    <q-card-section>
      <div class="row">
        <div class="col-6">
          <p>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod
            tempor incididunt ut labore et dolore magna aliqua.
          </p>
        </div>
        <div class="col-6" style="font-size: 18px;" >
          <p><strong class="personalInformationLabel">Age</strong> {{ age }}</p>
          <p><strong class="personalInformationLabel">Residence</strong> {{ residence }}</p>
          <p><strong class="personalInformationLabel">Address</strong> {{ address }}</p>
          <p><strong class="personalInformationLabel">e-mail</strong> {{ email }}</p>
          <p><strong class="personalInformationLabel">Phone</strong> {{ phone }}</p>
        </div>
      </div>
    </q-card-section>
  </q-card>
</template>

<script>
export default {
  name: 'AboutMe',
  data() {
    return {
      age: '26',
      residence: 'ITA',
      address: 'Desio(MB)',
      email: 'angelo.iossa.work@gmail.com',
      phone: '+39 3342071004'
    }
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

.about-me {
  color: white;
  font-size: 30px;
  font-family: poppins, Helvetica, sans-serif;
}
.personalInformationLabel {
  color: rgb(68, 148, 136);
}
</style>
