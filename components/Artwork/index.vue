<template>
  <section class="artwork">
    <canvas class="artwork__canvas" ref="canvas"></canvas>
  </section>
</template>

<script>
import ArtworkGL from './js/ArtworkGL'
import EventBus from '~/utils/event-bus'

export default {
  name: 'artwork',
  data () {
    return {

    }
  },
  mounted () {
    if (!this.artworkGL) {
      this.artworkGL = new ArtworkGL({
        $canvas: this.$refs.canvas
      })
    }
    EventBus.$emit('TRANSITION', this.$route.name)
  },
  watch: {
    '$route.name': function (_new, _old) {
      EventBus.$emit('TRANSITION', _new)
    }
  }
}
</script>

<style>
.artwork {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: #eaf2f5;
}
</style>
