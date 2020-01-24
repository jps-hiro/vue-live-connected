<template>
  <div id="app">
    <section class="hero is-fullheight">
      <hooper :autoPlay="true" :playSpeed="2000" :wheelControl="false">
      <slide>
        <video src="./assets/video/hero1.mp4" loop muted autoplay></video>
        <!-- <h1 class="slide">Work</h1> -->
      </slide>
      <slide>
        <img src="./assets/img/hero_3.jpg" alt="">
      </slide>
      </hooper>
    </section>

    <section class="live-welcome">
      <div class="container" style="margin-top: 50px;">
        <div class="columns is-multiline">
          <div class="column is-6 live-welcome--left">
            <h1 class="title">Welcome To Our Island</h1>
            <p>Discover what makes Ketchikan a Primere Alaskan Location For Remote Work. We have all the things someone needs to work remotely. From Highspeed Internet that has speeds that match or even beat the Lower 48, as well as amazing outdoor activities, top notch medical facilities, affordable renewable energy, among many other benifits. We are also a relatily short flight to and from Seattle allowing you to be able to acess all Alaska has to offer while still being close to other major cities via Alaska Air makes Ketchikan a perfect spot for remote working.</p>
            <img src="./assets/img/img1.jpg" alt="">
          </div>
          <div class="column is-6 live-welcome--right">
            <img src="./assets/img/img2.jpg" alt="">
          </div>
        </div>
      </div>

    </section>

    <!-- END WELCOME SECTION -->

    <section class="section hero live-video-hero has-text-white">
      <div class="center-box">
              <a href="https://vimeo.com/278261626" data-lity><div class="play-triangle"></div></a>
            <h1>WATCH THE STORY</h1>
      </div>
    </section>
    <!-- KETCHIKAN LIVE CONNECTED SECTION -->
    <section class="live-connected">
      <div class="container is-fluid">
        <div class="columns is-multiline">
          <div class="column is-12">
            <div class="rectangle"></div>
          </div>
          <div class="column is-7">
            <h1 class="main-header">KETCHIKAN: LIVE CONNECTED</h1>
            <h6 class="sub-header">For remote workers and other tech-based entrepreneurs, Ketchikan represents a unique opportunity to live a connected lifestyle.</h6>
            <p>Living in Ketchikan means living connected: to stunning natural beauty; to lightening-speed internet; to low-cost renewable energy; to unique arts and cultural experiences; and to excellent medical and educational facilities.</p>
            <p>Our residents enjoy an affordable and unparalleled quality of life with diverse economic opportunities and amazing cultural diversity in one of the world’s most beautiful settings for outdoor recreation.</p>
          </div>
          <div class="column is-5">
            <img src="./assets/img/ak_map.png" alt="Ketchikan Alaska Location">
          </div>
        </div>
      </div>
    </section>
    <!-- WORK PLAY HERO -->
      <section class="section hero work-play-hero">
        <h1 class="main-header has-text-white">EVERYTHING YOU NEED TO INNOVATE & SUCCEED IN BOTH WORK AND PLAY - <br>LIVES HERE</h1>
      </section>

    <!-- AMINITIES CARDS -->
<div class="amenities-header">
    <div class="container is-fluid">
      <div class="columns is-multiline">
        <div class="column is-12">
          <div class="rectangle"></div>
        </div>
        <div class="column is-12">
          <h1 class="main-header">Amenities</h1>
        </div>
      </div>
    </div>
</div>

    <aminities></aminities>



    <!-- WATCH STORY -->

      <section class="section hero live-video-hero2 has-text-white">
    <div class="center-box">
      <a href="https://vimeo.com/278264990" data-lity><div class="play-triangle"></div></a>
      <h1>WATCH THE STORY</h1>
    </div>
  </section>


  </div>
</template>

<script>
import { Hooper, Slide } from 'hooper';
import 'hooper/dist/hooper.css';
import Aminities from './components/Amenities';

export default {
  name: 'App',
  components: {
    Hooper,
    Slide,
    Aminities
  }
};
</script>

<style lang="css" src=""></style>

<style lang="scss" src="./assets/scss/app.scss"></style>
