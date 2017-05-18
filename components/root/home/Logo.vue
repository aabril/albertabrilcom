<template>
  <div class="Logo">
    <img src="~static/logo.png"></img>
  </div>
</template>

<script>
export default {
  props: [ ],
  layout: 'default' // you can set a custom layout for the error page
}
</script>

<style lang="less">
.Logo {
  img {
    max-width: 140px;
    margin: 30px;
  }
}
</style>
