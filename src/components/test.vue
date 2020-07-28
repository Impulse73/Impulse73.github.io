<template>
  <div class="main">
    <q-layout view="hHh Lpr lff" class="shadow-1">
      <Header />
      <LeftSideBar />
      <q-page-container>
        <q-page>
          <block1 />
          <Statictics />
          <howToStudy />
          <firstLesson />
        </q-page>
      </q-page-container>
    </q-layout>
  </div>
</template>
<style >
.main {
  margin-right: 10%;
  max-width: 1600px;
}
</style>
<script>
import howToStudy from './howToStudy'
import firstLesson from './firstLesson'
import Header from "./HeaderAndSideBar/Header"
import block1 from "./block1";
import Statictics from "./Statictics";
import LeftSideBar from "./HeaderAndSideBar/LeftSideBar";
export default {
  components: { /*SideBar*/ Header, LeftSideBar, block1, Statictics, howToStudy,firstLesson },
  data() {
    return {
      drawer: false,
      menuList: [],
    };
  },
  methods: {},
  beforeMount() {
    this.menuList = this.$store.getters.getListSideBar;
  },
};
</script>