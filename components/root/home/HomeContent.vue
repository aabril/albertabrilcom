<template>
  <div class="HomeContent">
    <Logo/>
    <div class="content">
      <h1 class="title">albert abril</h1>
      <div class="subtitle">
        Albert is a web developer based in London helping startups and digital studios to design web systems. With experience in PHP and Python and focused in JavaScript, from APIs to Single Page Applications.
      </div>
    </div>
  </div>
</template>

<script>
import Logo from '~/components/root/home/Logo.vue'
import VideoBG from '~/components/root/home/VideoBG.vue'

export default {
  components: { Logo, VideoBG },
  props: [ ],
  layout: 'default'
}
</script>

<style lang="less" scoped>
@import url('https://fonts.googleapis.com/css?family=Montserrat:700|Raleway:400');

.HomeContent {
  font-family: 'Raleway', sans-serif;
  height: 100vh;
  .content {
    width: 600px;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    margin-top: 6px;
    justify-content: center;
    h1.title {
      font-family: Montserrat, "Helvetica Neue", "Lucida Grande", Arial, Verdana, sans-serif;
      font-size: 100px;
      font-weight: 700;
      line-height: 0.7;
      margin: 0 0 1.5rem 0;
      color: #000000; 
      -webkit-font-smoothing: antialiased;
    }
    .subtitle {
      font-family: "Raleway", "Helvetica Neue", "Lucida Grande", Arial, Verdana, sans-serif;
      font-size: 15px;
      font-weight: 400;
      line-height: 1.8;
      color: #6d6d6d;
      margin-top: 2.8rem;
      -webkit-font-smoothing: antialiased;
    }
  }
}
</style>
