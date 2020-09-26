<template>
  <div id="app">
    <navbar/>
    <Topbanner/>
    <Serverinfo/>
    <!--<HelloWorld/>-->
  </div>
</template>

<script lang="ts">
import { Component, Vue } from "vue-property-decorator";
import navbar from "./components/navbar.vue";
import Topbanner from "./components/Topbanner.vue";
import Serverinfo from "./components/Serverinfo.vue";
/*import HelloWorld from "./components/HelloWorld.vue";*/

@Component({
  components: {
    navbar,
    Topbanner,
    Serverinfo,
    /*HelloWorld,*/
  }
})
export default class App extends Vue {}
</script>

<style>
* {
  padding: 0px;
  border: 0px;
  margin: 0px;
  box-sizing: border-box;
}
section {
  height: 100vh;
}
</style>
