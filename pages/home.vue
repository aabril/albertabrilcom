<template>
  <div>
    <TopNav/>
    <HomeContent/>
    <SocialNav/>
  </div>
</template>

<script>
import HomeContent from '~/components/home/HomeContent.vue'
import TopNav from '~/components/home/TopNav.vue'
import SocialNav from '~/components/home/SocialNav.vue'

export default {
  components: { HomeContent, TopNav, SocialNav },
  props: [ ],
  layout: 'default' // you can set a custom layout for the error page
}
</script>
