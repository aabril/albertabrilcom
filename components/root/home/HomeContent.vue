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

export default {
  components: { Logo },
  props: [ ],
  layout: 'default'
}
</script>

<style lang="less" scoped>
@import url('https://fonts.googleapis.com/css?family=Montserrat:700|Raleway:200');

.HomeContent {
  font-family: 'Raleway', sans-serif;
  height: 100vh;
  .content {
    width: 600px;
    position: absolute;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);

    h1.title {
      font-family: Montserrat, "Helvetica Neue", "Lucida Grande", Arial, Verdana, sans-serif;
      font-size: 100px;
      font-weight: 700;
      line-height: 0.9;
      margin: 0 0 1.5rem 0;
      color: #000000; 
    }

    .subtitle {
      font-family: "Raleway", "Helvetica Neue", "Lucida Grande", Arial, Verdana, sans-serif;
      font-size: 15px;
      font-weight: 200;
      line-height: 1.8;
      color: #6d6d6d;

      margin-top: 3rem;
    }


  }
}
</style>
