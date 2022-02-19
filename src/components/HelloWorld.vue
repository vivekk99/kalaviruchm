<template>
  <div class="home">
    <SlideShow />
  </div>
</template>

<script>
import SlideShow from './SlideShow.vue';
export default {
  components: { SlideShow },
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.home{
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>
