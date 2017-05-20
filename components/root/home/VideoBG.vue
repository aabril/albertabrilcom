<template>
  <div class="VideoBG">
      <video class="video" autoplay loop>
          <source :src="video_webm"  type='video/webm; codecs="vp8, vorbis"' />
          <source :src="video_mp4" type='video/mp4; codecs="avc1.42E01E, mp4a.40.2"' />
          <source :src="video_ogv" type='video/ogg; codecs="theora, vorbis"' />
          <img src="/static/video-background.jpg">
          <div class="grid"></div>
      </video>
  </div>
</template>

<script>
export default {
  props: [ ],
  layout: 'default',
  data () {
    return {
      'video_mp4': 'https://doc-04-1c-docs.googleusercontent.com/docs/securesc/98c4aivmrlgv6ssvk0erf6ptndblp478/n5il9ivid99j0l5upgs0ctsmmqfoii1j/1495224000000/08897849265195409924/08897849265195409924/0B2IziBCKwg5AaHZfeEplLWJDVEk?e=download',
      'video_webm': 'https://doc-10-1c-docs.googleusercontent.com/docs/securesc/98c4aivmrlgv6ssvk0erf6ptndblp478/06b3o9d9oko4uo8p9i58k9hkh0koqab0/1495224000000/08897849265195409924/08897849265195409924/0B2IziBCKwg5AY1Z2UXRGQmNtNG8?e=download&nonce=gcbahcbv0uqno&user=08897849265195409924&hash=0gfl9nrkvl4qh0h563s5geg42flv8alq',
      'video_ogv': ''
    }
  }
}
</script>

<style lang="less">
.VideoBG {
  .video-container {
    height: 400px;
    width: 100%;
    position: relative;
    overflow-x: hidden;
    color: #fff;
  }

  .video {
    position: fixed;
    top: 50%;
    left: 50%;
    z-index: -1;
    min-width: 100%;
    min-height: 100%;
    width: auto;
    height: auto;
    transform: translate(-50%, -50%);
  }

  .grid {
    background: url(https://i.stack.imgur.com/hqR7r.png);
    width: 100%;
    height: 100vh;
    z-index: 1000;
  }

}
</style>
