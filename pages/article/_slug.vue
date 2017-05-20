<template>
  <div>
    <h2>article</h2>
    <h2>$route.params.slug: {{ $route.params.slug }}</h2>
    <h2>slug: {{ slug }}</h2>
  </div>
</template>

<script>
export default {
  components: {},
  data () {
    return {
      slug: this.$route.params.slug
    }
  },
  created () {
    // console.log(this.$route.params.slug)
    // console.log(this)
  }
}
</script>
