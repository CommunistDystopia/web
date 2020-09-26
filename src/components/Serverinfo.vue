<template>
<section>

  <div class="grid">
  <div class="box">
    <div class="video_title"><strong>PLAY WITH US</strong></div>
  </div>

  <div class="box">
    <div class="videoWrapper">
      <iframe src="https://www.youtube.com/embed/pmanD_s7G3U" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
    </div>
  </div>

  <div class="box">
    <div class="info_box">
      <div class="information">
        <h1>INFORMATION</h1>
        <p class="info_text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. </p>
        <p class="info_text"> Curabitur nec nulla vel tellus maximus sodales vel a magna. </p>
      </div>
        <img class="join_discord" src="../assets/join_discord.png" />
    </div>   
  </div>

  </div>

  <!--<h1 class="video_title">SOME TITLE</h1>-->
  <!--<div class="row">
  <div class="videoWrapper col-8">
  <iframe src="https://www.youtube.com/embed/pmanD_s7G3U" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
  </div>
  <div class="info_box col-4">
    <div class="information">
      <h1>INFORMATION</h1>
      
      <p class="info_text">Lorem ipsum dolor sit amet, consectetur adipiscing elit. </p>
      <p class="info_text"> Curabitur nec nulla vel tellus maximus sodales vel a magna. </p>
  </div>
  <img class="join_discord" src="../assets/join_discord.png" />
  </div>
  </div>-->
</section>
</template>

<script lang="ts">
import { Component, Prop, Vue } from "vue-property-decorator";

@Component
export default class Serverinfo extends Vue {
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

section {
  width: 100%;
  display: flex;
  justify-content: space-around;
  flex-flow: row wrap;
  background-color: #343333;
}

.info_box {
    padding: 10px;
    margin-top: 10px;
}

h1 {
  text-shadow: 3px 4px 5px rgb(0, 0, 0);
  color: rgb(255, 255, 255);
  padding: 10px;
}

.info_text{
  color: rgb(255, 255, 255);
}

.join_discord {
  display:block;
  margin:auto;
}

.video_title {
  display: block;
  color: aliceblue;
  text-align: left;
  margin: 20px 20px 0px 20px;
  font-size: 20px;
}

.videoWrapper {
  position: relative;
  padding-bottom: 56.25%; /* 16:9 */
  width: 100%;
}

.videoWrapper iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  padding: 20px 10px 10px 10px;
  margin-top: 10px;
}

/*Small Screen*/
@media screen and (min-width: 200px) and (max-width: 375px){

.information{
    display:block;
    border: 2px solid black;
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.705);
}

.info_text{
  font-size: 22px;
  padding: 10px;
}

.join_discord {
  margin-top: 10px;
  width: 70%;
}

}

/*Middle Screen*/
@media screen and (min-width: 375px) and (max-width: 767px){

.information {
  display:block;
  border: 2px solid black;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.705);
  width: 100%;
}

h1 {
  text-shadow: 3px 4px 5px rgb(0, 0, 0);
  color: rgb(255, 255, 255);
  padding: 10px;
  font-size: 26px;
}

.info_text{
  font-size: 24px;
  padding: 15px;
}

.join_discord {
  margin-top: 20px;
  width: 50%;
}

}

/*Large Screen*/
@media screen and (min-width: 768px){

.grid {
  display: grid;
  width: 100%;
  grid-template-columns: max-content auto max-content max-content;
  grid-template-rows: max-content auto;
  grid-gap: 15px;
  padding: 15px;
}

.box:nth-child(1) {
grid-column: 1/5;
}


.box:nth-child(2) {
  grid-column: 1/4;
}


.box:nth-child(3) {
  grid-column: 4/5;
}

.videoWrapper iframe {
  padding: 10px 10px 10px 10px;
  margin-top: 0px;
}

.info_box {
    padding: 10px;
    width: 300px;
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.705);
}

.info_text{
  font-size: 18px;
  padding: 15px;
}

.join_discord {
  margin-top: 10px;
  width: 50%;
}


/*.grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: repeat(2, 1fr);
  grid-gap: 15px;
  padding: 15px;
}

.box {
  display: flex;
  justify-content: center;
  align-items: center;
  color: black;
}

.box:nth-child(1) {
  grid-column: 1/4;
  grid-row: span 3;
  background-color: rgb(0, 92, 95);
}


.box:nth-child(2) {
  grid-column: 1/2;
  background-color: darkcyan;
}


.box:nth-child(3) {
  grid-column: 2/4;
  grid-row: 2/3;
  background-color: darkgoldenrod;
}*/


/*.info_text{
  font-size: 18px;
  padding: 15px;
}

.video_title{
  background-color: aqua;
}

.videoWrapper {
  position: relative;
  padding-bottom: 56.25%; /* 16:9 */
  /*width: 66.66%;
  height: auto;
  margin-top: 90px;
}

.videoWrapper iframe {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  padding: 20px 10px 10px 10px;
}

.join_discord {
  margin-top: 20px;
  width: 40%;
}*/

}
</style>