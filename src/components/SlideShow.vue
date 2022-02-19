<template>
   <div class="slide-Show">
    <b-carousel
      id="carousel-1"
      v-model="slide"
      :interval="3000"
      controls
      indicators
      background="#ccc"
      style="text-shadow: 1px 1px 2px #000;"
      @sliding-start="onSlideStart"
      @sliding-end="onSlideEnd"
    >
      <!-- Text slides with image1 -->
      <b-carousel-slide
        caption=""
        text=""  
      >
      <template v-slot:img>
          <img
            class="d-block img-fluid w-100"
            src="@/assets/images/44.jpg"
            alt="image slot"
          >
        </template>
      </b-carousel-slide>
<!-- Text slides with image2 -->
      <b-carousel-slide
        caption=""
        text=""  
      >
      <template v-slot:img>
          <img
            class="d-block img-fluid w-100"
            src="@/assets/images/122.jpg"
            alt="image slot"
          >
        </template>
      </b-carousel-slide>

<!-- Text slides with image3 -->
      <b-carousel-slide
        caption=""
        text=""  
      >
      <template v-slot:img>
          <img
            class="d-block img-fluid w-100"
            src="@/assets/images/122.jpg"
            alt="image slot"
          >
        </template>
      </b-carousel-slide>

<!-- Text slides with image4 -->
      <b-carousel-slide
        caption=""
        text=""  
      >
      <template v-slot:img>
          <img
            class="d-block img-fluid w-100"
            src="@/assets/images/332.jpg"
            alt="image slot"
          >
        </template>
      </b-carousel-slide>

      <!-- Text slides with image5 -->
      <b-carousel-slide
        caption=""
        text=""  
      >
      <template v-slot:img>
          <img
            class="d-block img-fluid w-100"
            src="@/assets/images/266.jpg"
            alt="image slot"
          >
        </template>
      </b-carousel-slide>
     
      
    </b-carousel>
  </div> 
</template>
<script>
export default {
    name:'SlideShow',
     data() {
      return {
        slide: 0,
        sliding: null
      }
    },
    methods: {
      onSlideStart() {
        this.sliding = true
      },
      onSlideEnd() {
        this.sliding = false
      }
    }
}
</script>
<style scoped>
.slide-Show{
    width: 60%;
    margin-top: 30px;
}

</style>
