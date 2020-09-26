<template>
<section>
  <div>
    <img class="topbannerimg" alt="Vue logo" src="../assets/topbanner_image.png" />
  </div>
</section>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class HelloWorld extends Vue {
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

.topbannerimg {
  display:flex;
  width:100%;
  height:100%;
  background-color:transparent;
}
</style>
