<template>
  <q-card flat bordered class="my-card absolute-right q-pa-xl" style="overflow: auto;">
    <q-card-section>
      <span class="about-me"><strong>Contact</strong></span>
    </q-card-section>

    <q-card-section>
      <div class="row">
        <div class="col-4">
          <p>
            <q-card flat class="cardsContact text-center q-mb-md">
              <q-card-section>
                <i class="fa-solid fa-location-dot fa-2xl iconStyle" style="margin-top: 20px;"></i>
                <p class="q-mt-lg q-mb-sm">{{ address }}</p>
              </q-card-section>
            </q-card>
            <q-card flat class="cardsContact text-center q-mb-md">
              <q-card-section>
                <i class="fa-solid fa-phone fa-2xl iconStyle" style="margin-top: 20px;"></i>
                <p class="q-mt-lg q-mb-sm">{{ phone }}</p>
              </q-card-section>
            </q-card>
            <q-card flat class="cardsContact text-center q-mb-md">
              <q-card-section>
                <i class="fa-solid fa-envelope fa-2xl iconStyle" style="margin-top: 20px;"></i>
                <p class="q-mt-lg q-mb-sm">{{ email }}</p>
              </q-card-section>
            </q-card>
            <!-- <q-card flat class="cardsContact text-center q-mb-md">
              <q-card-section>
                <i class="fa-brands fa-instagram fa-2xl iconStyle" style="margin-top: 20px;"></i>
                <p class="q-mt-lg q-mb-sm">Prima card</p>
              </q-card-section>
            </q-card> -->
          </p>
        </div>
        <div class="col-8" style="font-size: 18px;">

        </div>
      </div>
    </q-card-section>
  </q-card>
</template>

<script>
export default {
  name: 'Contact',
  data() {
    return {
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

.cardsContact {
  background-color: rgb(68,68,68);
}

.iconStyle {
  color: rgb(68, 148, 136);
  font-size: 35px;
}
</style>

