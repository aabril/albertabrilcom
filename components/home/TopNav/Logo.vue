<template>
  <img class="brand-logo" src="~static/logo.png"></img>
</template>

<script>
export default {
  props: [ ],
  layout: 'default' // you can set a custom layout for the error page
}
</script>

<style>
.brand-logo {
  position: absolute; 
  top: 30px;
  left: 30px;
  max-width: 140px;
}
</style>
