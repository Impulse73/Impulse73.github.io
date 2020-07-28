<template>
  <div>
    <q-header style="background-color: white; max-widht: 1600px;">
      <q-toolbar>
        <q-toolbar-title class="headerTitle q-pa-md" style="color: black">
          <img src="../../assets/logo1.jpg" alt="logo">
          <img src="../../assets/textlogo.jpg" alt="logo">
        </q-toolbar-title>
        <q-btn class="headerBtn text-h6" color="yellow" text-color="black" label="Хочу на обучение" />
      </q-toolbar>
    </q-header>
  </div>
</template>
<style>
  .headerTitle {
    margin-left: 10%;
  }  
  .headerTitle img {
    height: 70px;
    max-width: 200px;
  }
  .headerBtn {
    margin-right: 10%;
  }
  .imgHeader {
    height: 50px;
    max-width: 50px;
  }
</style>
<script>
import { QBtn } from "quasar";
export default {
  components: { QBtn },
  data() {
    return {};
  },
  methods: {},
};
</script>
