<template>
  <div>
    <div v-if="!ready">
      <Loading/>
    </div>
    <div v-if="ready">
      <MenuNav/>
      <HomeContent/>
      <SocialNav/>
    </div>
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
