<template>
  <div class="column items-center q-ml-lg">
    <div class="col">
      <q-btn @click="showHome()" icon="home" class=".self-center control" size="20px" round />
      <q-tooltip anchor="center left" self="center end" >Home</q-tooltip>
    </div>
    <div class="col">
      <q-btn @click="showAboutMe()" icon="person" class="q-mt-md .self-center control" size="20px" round />
      <q-tooltip anchor="center left" self="center end" >About me</q-tooltip>
    </div>
    <div class="col">
      <q-btn @click="showResume()" icon="school" class="q-mt-md .self-center control" size="20px" round />
      <q-tooltip anchor="center left" self="center end" >Resume</q-tooltip>
    </div>
    <div class="col">
      <q-btn @click="showContact()" icon="mail" class="q-mt-md .self-center control" size="20px" round />
      <q-tooltip anchor="center left" self="center end" >Contact</q-tooltip>
    </div>
  </div>
</template>

<script>
export default {
  // name: 'ComponentName',
  data() {
    return {}
  },
  methods: {
    showHome() {
      this.$emit('showHome');
    },
    showAboutMe() {
      this.$emit('showAboutMe');
    },
    showResume() {
      this.$emit('showResume');
    },
    showContact() {
      this.$emit('showContact');
    },
  }
}
</script>
<style>
.control {
  background-color: #757575;
  color: rgb(68, 148, 136);
}
</style>
