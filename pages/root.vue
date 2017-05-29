<template>
  <div>
    <div v-if="!ready">
      <Loading/>
    </div>
    <transition name="fade">
      <div v-if="ready">
        <MenuNav/>
        <HomeContent/>
        <SocialNav/>
      </div>
    </transition>
  </div>
</template>

<script>
import Loading from '~/components/root/common/Loading.vue'

import HomeContent from '~/components/root/home/HomeContent.vue'
import SocialNav from '~/components/root/common/SocialNav.vue'
import MenuNav from '~/components/root/common/MenuNav.vue'

export default {
  components: { Loading, SocialNav, HomeContent, MenuNav },
  props: [ ],
  layout: 'default',
  data () {
    return {
      ready: false
    }
  },
  mounted () {
    this.ready = true
  }
}
</script>

<style scoped>
.fade-enter-active, .fade-leave-active {
  transition: opacity 2.4s
}
.fade-enter, .fade-leave-to /* .fade-leave-active in <2.1.8 */ {
  opacity: 0
}
</style>
