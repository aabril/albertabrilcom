<template>
  <div>
    <Logo/>
    <MenuButton/>
  </div>
</template>

<script>
import Logo from '~/components/home/TopNav/Logo.vue'
import MenuButton from '~/components/home/TopNav/MenuButton.vue'

export default {
  props: [ ],
  layout: 'default', // you can set a custom layout for the error page
  components: { Logo, MenuButton }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Montserrat:600|Raleway');
body {
  font-family: 'Raleway', sans-serif;
}
.content {
  border: 1px solid black;
  height: 60px;
}
</style>
