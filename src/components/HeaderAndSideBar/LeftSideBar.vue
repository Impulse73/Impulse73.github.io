<template>
        <q-drawer
        class="drawer"
        v-model="drawer"
        show-if-above
        :width="400"
        :breakpoint="800"
        bordered
      >
          <q-list class="list" v-for="(menuItem, index) in menuList" :key="index">
            <q-item  class="itemList" clickable :active="menuItem.title === 'Outbox'" v-ripple>
              <q-item-section avatar>
                <q-icon  color="yellow-8" class="icons" :name="menuItem.image" />
              </q-item-section>
              <q-item-section class="text-h6">
                {{ menuItem.title }}
              </q-item-section>
            </q-item>
           <q-separator v-if="menuItem.separator" />

          </q-list>
      </q-drawer>
</template>
<style>
  .drawer {
    padding-left: 10%;
  }
  .list {
     margin-left: 30%;
  }
  .itemList {
    height: 80px;
  }
</style>
<script>

import {QSeparator} from 'quasar'
export default {
    components : {QSeparator},
  data () {
    
    return {
      drawer: false,
      menuList: []

    }
  },
  methods : {

  },
  beforeMount() {
    this.menuList = this.$store.getters.getListSideBar
  }
}
</script>