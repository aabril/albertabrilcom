<template>
  <div>
    <HomeContent/>
    <SocialNav/>
  </div>
</template>

<script>
import HomeContent from '~/components/root/home/HomeContent.vue'
import SocialNav from '~/components/root/common/SocialNav.vue'

export default {
  components: { SocialNav, HomeContent },
  props: [ ],
  layout: 'default' // you can set a custom layout for the error page
}
</script>
