<template>
  <div class="q-pa-md row items-start q-gutter-md justify-center">
      <h3 class="text-h3 text-weight-bolder">Как мы обучаем</h3>
    <q-card class="card0">
      <q-card-section class="bg-grey-3 text-black">
        <div class="text-h4 text-weight-bold">Методика обучения</div>
        <div class="text-subtitle1">{{contentText[0].text}}</div>
      </q-card-section>
    </q-card>
     <q-card class="card1">
      <q-card-section class="bg-purple-13 text-white">
        <div class="text-h4 text-weight-bold">Формирование групп</div>
        <div class="text-subtitle1">{{contentText[1].text}}</div>
      </q-card-section>
    </q-card>
     <q-card class="howToStudyCardrow">
      <q-card-section class="bg-indigo-12 text-white">
        <div class="text-h4 text-weight-bold">Аттестация</div>
        <div class="text-subtitle1">{{contentText[3].text}}</div>
      </q-card-section>
    </q-card>
     <q-card class="howToStudyCardrow">
      <q-card-section class="bg-grey-1 text-black">
        <div class="text-h4 text-weight-bold">Проверка работ</div>
        <div class="text-subtitle1">{{contentText[4].text}}</div>
      </q-card-section>
    </q-card>
     <q-card class="howToStudyCardthirdrow">
      <q-card-section class="bg-green-14 text-white">
        <div class="text-h4 text-weight-bold">Программа</div>
        <div class="text-subtitle1">{{contentText[2].text}}</div>
      </q-card-section>
    </q-card>
     <q-card class="howToStudyCardthirdrow">
      <q-card-section class="bg-amber-14 text-white">
        <div class="text-h4 text-weight-bold">Ивенты</div>
        <div class="text-subtitle1">{{contentText[5].text}}</div>
      </q-card-section>
    </q-card>
  </div>
</template>

<style>
    .card1{
        width: 100%;
        max-width: 300px;
    }
    .howToStudyCard {
        width: 100%;
        max-width: 500px;
    }
    .howToStudyCardrow{
        width: 100%;
        max-width: 400px;
    }
    .card0 {
        width: 100%;
        max-width: 500px;
    }
    .howToStudyCardthirdrow {
         width: 100%;
        max-width: 400px;
    }
</style>
<script>
import { QCard, QCardSection,   } from "quasar";
export default {
  components: { QCard, QCardSection,   },
  data() {
    return {
      contentText: [],
    };
  },
  methods: {},
  beforeMount() {
    this.contentText = this.$store.getters.getHowToStudyText;
  },
};
</script>