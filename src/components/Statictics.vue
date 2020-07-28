<template>
  <div class="q-pa-xl">
    <div id="row" class="q-pa-xs row items-start q-gutter-md justify-center">
      <q-card  class="my-card">
        <q-card-section>
          <div class="cardItem col">
            <img src="../assets/rocket.png" />
            <p>8 лет в сфере образования</p>
          </div>
        </q-card-section>
      </q-card>
      <q-card class="my-card">
        <q-card-section>
          <div class="col">
            <img src="../assets/womanStudent.png" />
            <p>117 филиалов по всей России</p>
          </div>
        </q-card-section>
      </q-card>
      <q-card class="my-card">
        <q-card-section>
          <div class="col">
            <img src="../assets/oneHundreed.png" />
            <p>Выпускаем 100-бальников каждый год</p>
          </div>
        </q-card-section>
      </q-card>
    </div>
  </div>
</template>
<style>
#row p {
  text-align: center;
  font-size: 1.3rem;
  font-family: system-ui;
}
#row img {
  padding-left: 25%;
}
.my-card {
  width: 100%;
  max-width: 265px;
  max-height: 260px;
}
</style>
<script>
import { QCard, QCardSection } from "quasar";
export default {
  components: { QCard, QCardSection },
  data() {
    return {};
  },
};
</script>