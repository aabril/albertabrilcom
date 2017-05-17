<template>
  <div>
    <TopNav/>
    <HomeContent/>
    <SocialNav/>
  </div>
</template>

<script>
import HomeContent from '~/components/HomeContent.vue'
import TopNav from '~/components/TopNav.vue'
import SocialNav from '~/components/SocialNav.vue'

export default {
  components: { HomeContent, TopNav, SocialNav },
  props: [ ],
  layout: 'default' // you can set a custom layout for the error page
}
</script>

