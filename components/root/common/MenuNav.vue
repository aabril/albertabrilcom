<template>
<ul class="MenuNav" @click="onClick">
  <li :class="[isActive ? 'ion-close-round rotating rotated' : 'ion-navicon-round rotating' ]" data-pack="default" data-tags="menu, hamburger, slide menu"></li>
</ul>
</template>

<script>
// import TWEEN from 'https://unpkg.com/tween.js@16.3.4'

export default {
  props: [ ],
  layout: 'default',
  data () {
    return {
      'isActive': false
    }
  },
  methods: {
    onClick () {
      this.isActive = !this.isActive
    }
  }
}
</script>

<style lang="less" scoped>
@import 'http://code.ionicframework.com/ionicons/2.0.1/css/ionicons.min.css';

.MenuNav {
  position: absolute;
  top: 30px;
  right: 30px;
  li {
    font-size: 33px;
  }

  .rotating { 
      -webkit-transition: all 0.3s ease-in-out;
      -moz-transition: all 0.3s ease-in-out;
      -o-transition: all 0.3s ease-in-out;
      transition: all 0.3s ease-in-out;
  }

  .rotated { 
      opacity: 1;
      background: white;
      transform: rotate(-180deg); 
      -webkit-transform: rotate(-180deg); 
      -moz-transform: rotate(-180deg); 
      -o-transform: rotate(-180deg); 

      -webkit-transition: all 0.3s ease-in-out;
      -moz-transition: all 0.3s ease-in-out;
      -o-transition: all 0.3s ease-in-out;
      transition: all 0.3s ease-in-out;


      // transform: translate(-150px,0) rotate(180deg); 
      // -webkit-transform: translate(-150px,0) rotate(180deg); 
      // -moz-transform: translate(-150px,0) rotate(180deg); 
      // -o-transform: translate(-150px,0) rotate(180deg); 
  }

}
</style>
