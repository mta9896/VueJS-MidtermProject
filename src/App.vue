<template>
  <!-- Don't drop "q-app" class -->
  <div class="background">
    <!--<img src="statics/background.jpg">-->
    <div class="toolbar">
      <div class="toolbarButtons">
        <q-btn>
          ورود
        </q-btn>
        <q-btn class="signupButton">
          ثبت نام
        </q-btn>
      </div>
      <div class="toolbarTitle">
        <i class="material-icons">account_circle</i>
        امیرکبیر استودیو
      </div>
    </div>
    <div class="page-title">
      <div class="main-page-title">
     مرکز بازی سازی امیرکبیر
      </div>
      <div class="page-title-discription">
لورم ایپسوم
      </div>
      <div class="page-title-buttons">
        <q-btn class="show-trailer-button">
          <i class="material-icons">account_circle</i>
          تریلر این بازی
        </q-btn>
        <q-btn class="enter-game-button">
          ورود به صفحه بازی
        </q-btn>
      </div>

    </div>
    <div class="slider-container">
        <q-card class="slider-item"  v-for="item in sliderItems">
            <img class="slider-image" @click="changeBackGround(item.image)" :src="item.image">
            <div class="image-caption">
            {{ item.message }}
            </div>

          <!--</q-card>-->
        </q-card>

    </div>
  </div>
</template>
<script>
  import axios from 'axios'
   import {
     QLayout,
     QToolbar,
     QBtn,
     QCard
  } from 'quasar'

  export default {
    components: {
      QLayout,
      QToolbar,
      QBtn,
      QCard
    },
    data() {
      return {
        message: 'Hello Vue!',
        sliderItems: [
          { message: 'بازی اول',
            image: 'statics/1.jpg'},
          { message: 'بازی دوم',
            image: 'statics/2.jpg'},
          { message: 'بازی سوم',
            image: 'statics/3.jpg'},
          { message: 'بازی چهارم',
            image: 'statics/4.jpg'},
          { message: 'بازی پنجم',
            image: 'statics/5.jpg'}
        ]
      }
    },

    methods: {
      async foo() {
        axios.get('laksdjf').then((response)=> {

        })
        let response = await axios.get('ljsdf')
      },

      changeBackGround(imgUrl){
        console.log(imgUrl);
        let arg = "url('"+imgUrl+"\')";
        console.log(arg);
        document.body.style.background = arg;
      }
    }
  }
</script>


<style lang="stylus">
  @import 'statics/font-face.css';
body
  background:url(statics/1.jpg)
  font-family "Shabnam"

.background
  display flex
  flex-direction column
  background-color rgba(0, 0, 0, 0.5)
  color white
  position absolute
  top 0
  left 0
  width 100%
  height 100%
.toolbar
  display flex
  flex-direction row
  padding-top 1%

.toolbarTitle, .toolbarButtons
  width 50%
  text-align center

.signupButton
  background-color #2f77a6
.page-title
  flex-grow 2
  /*background-color darkorange*/
  display flex
  flex-direction column
  padding-right  22%
  align-items flex-end
  justify-content center
.main-page-title
  font-size 2em
.page-title-discription
  font-size 1em
  font-family "Shabnam"

.page-title-discription, .page-title-buttons
  margin-top 3%

.enter-game-button
  background-color #2f77a6
  font-size inherit
.show-trailer-button
  font-size inherit
.page-title-buttons, .page-title-discription
  font-size 1.2em

.slider-item
  background-color #2f77a6
.slider-item:hover img
  opacity 0.3
  width 23vw
  height 25vh

.slider-container
  /*background-color darkorange*/
  flex-grow 1
  display flex
  flex-direction row-reverse
  justify-content space-around
  align-items center

.slider-image
  width 18vw
  height 20vh

.image-caption
  text-align right
  padding-right 5%
  padding-bottom 2%
</style>
