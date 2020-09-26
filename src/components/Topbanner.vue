<template>
<section class="section_container">
 
  <div class="banner_title">Communist Dystopia</div>
  
  <div class="play_box play_now">
    <img class="hammerimg" src="../assets/hammer_and_sickle.png" /> Communistsomalia.serv.nu <img class="hammerimg" src="../assets/hammer_and_sickle.png" />
  </div>
  
</section>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class Topbanner extends Vue {
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

@font-face {
	font-family: 'Conv_MinecrafterReg';
	src: url('../assets/fonts/MinecrafterReg.eot');
	src: local('MinecrafterReg'), 
  url('../assets/fonts/MinecrafterReg.woff') format('woff'), 
  url('../assets/fonts/MinecrafterReg.ttf') format('truetype'), 
  url('../assets/fonts/MinecrafterReg.svg') format('svg');
	font-weight: normal;
	font-style: normal;
}

 .section_container {
  display: flex;
  flex-flow: column wrap;
  justify-content: space-around;
  align-items: center;
  background-image: url(../assets/topbanner_image.png);
  background-position: center center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;
}
.section_container:before {
	content:'';
	position: absolute;
  top: 0;
	bottom: 0;
	left: 0;
	right: 0;
	background-color: rgba(59, 53, 53, 0.6);
}

.banner_title {
  font-size: 40px;
  text-align: center;
  font-family: 'Conv_MinecrafterReg';
  color: #BD0000;
  -webkit-text-stroke-width: 3px;
  -webkit-text-stroke-color: rgb(19, 13, 13);
  text-shadow:
       5px 7px 3px rgb(36, 36, 36);
  z-index: 30;
}

.play_now {
  order: 2;
  font-family: 'Conv_MinecrafterReg';
  text-align: center;
  font-size: 16px;
}

.play_box {
  border: 1px solid black;
  width: 100%;
  background-color: #F28300;
  padding: 10px;
  z-index: 30;
  box-shadow: 5px 8px 5px rgb(34, 34, 34);
}

@media screen and (min-width: 200px) and (max-width: 375px){

  .banner_title {
  font-size: 40px;
}

.play_now {
  font-size: 16px;
}

.hammerimg {
  display: none;
}

}

/*Mobile*/
@media screen and (min-width: 375px) and (max-width: 767px){

.banner_title {
  font-size: 54px;
}

.play_now {
  font-size: 22px;
}

.hammerimg {
  display: none;
}
}
/*PC*/
@media screen and (min-width: 768px) {

.banner_title {
  font-size: 60px;
}

.play_now {
  font-size: 32px;
}

.hammerimg{
  width: 50px;
  height: 50px;
}
}

/*
.banner_title {
  display: flex;
  flex-direction: column;
  justify-content: center;
  z-index: 30;

}
<img class="banner_title" src="../assets/Minecraft-Logo.png" align="middle"/>

.banner_section{
  display:flex;
  flex-flow: row wrap;
  justify-content: center;
}

.topbannerimg {
  width:100%;
  height:100%;
  background-color:transparent;
}

.play_now {
  text-align: center;
  font-size: 32px;
  width: 100%;
  background-color: rgb(251, 253, 99);
  z-index: 30;
}*/

/*
.banner_title {
  order: 1;
  position: absolute;
  background-color: transparent;
  width: 100%;
  height: auto;
  z-index: 30;
}*/
/*<div>
    <img src="../assets/logo.png" />
      <div class="banner_section">
        <img class="topbannerimg" alt="Vue logo" src="../assets/topbanner_image.png" />
        <span class="play_now">Communistsomalia.serv.nu</span>
      </div>
  </div>

  <div class="play_box">
      <span class="play_now">Communistsomalia.serv.nu</span>
  </div>
  
   */
</style>