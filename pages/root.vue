<template>
  <div>
    <MenuNav/>
    <HomeContent/>
    <SocialNav/>
  </div>
</template>

<script>
import HomeContent from '~/components/root/home/HomeContent.vue'
import SocialNav from '~/components/root/common/SocialNav.vue'
import MenuNav from '~/components/root/common/MenuNav.vue'

export default {
  components: { SocialNav, HomeContent, MenuNav },
  props: [ ],
  layout: 'default' // you can set a custom layout for the error page
}
</script>
