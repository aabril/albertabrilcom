<template>
  <p class="content">Home Content</p>
</template>

<script>
export default {
  props: [ ],
  layout: 'default' // you can set a custom layout for the error page
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
