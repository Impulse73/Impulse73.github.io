<template>
  <div class="sidebar" id="sidebar">
    <div class="sidebar_top">
      <div class="sidebar_top_logo">
        <img class="visible-sm" src="../assets/logo.png">
      </div>  
      <ul class="sidebar_top_list">
          <li
            v-for="(value, index) in listSideBar"
             :key="index">
             <div class="fit row inline ">
             <div class="image">
             <img style="max-width: 25px; margin-right: 20px" :src="value.image">
             </div>
             <div class="title" >
               {{value.title}}
             </div>
             </div>
          </li>
      </ul>
      {{this.images}}
    </div>
  </div>
 
</template>

<style>
  li {
  list-style: none;
  }
  .visible-sm {
    max-width: 50px;
  }
</style>

<script>
import {  } from 'quasar'
export default {
  name: 'SideBar',
  components: {  },  
   data () {
    return {
      images: [],
      listSideBar : [],
      left: false
    }
  },
  methods : {
    
  },
  beforeMount(){
    this.listSideBar = this.$store.getters.getListSideBar;
    this.images = this.listSideBar.image
  }
}
</script>
