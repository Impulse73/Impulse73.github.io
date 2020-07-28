<template>
    <div class="q-pa-xl">
         <q-field class="q-pa-xl" color="yellow" bg-color="yellow" rounded outlined>
        <template v-slot:control>
          <div class="self-center full-width no-outline text-h5 text-center text-weight-bold" tabindex="0">{{text}}</div>
        </template>
      </q-field>
      <q-field  borderless >
        <template v-slot:control>
          <div class="self-center full-width no-outline text-h5 text-center text-weight-bold" tabindex="0">{{feedback}}</div>
        </template>
      </q-field>
    </div>
</template>
<style>

</style>
<script>
import {QField} from 'quasar'
    export default {
        components: {
            QField
        },
        data () {
            return {
                text : "ПЕРВОЕ ЗАНЯТИЕ ПО ВСЕМ ПРЕДМЕТАМ - БЕСПЛАТНО",
                feedback: "Мы всегда на связи! Задай вопрос или запишись на обучение уже сегодня"


            }
        }
    }
</script>