<template>
  <div class="container">
    <div class="row">
      <div class="col-md-8">
        <b-carousel id="carousel1"
          style="text-shadow: 1px 1px 2px #333;"
          controls
          indicators
          background="#ababab"
          :interval="3000"
          img-width="865"
          img-height="412"
          v-model="slide"
          @sliding-start="onSlideStart"
          @sliding-end="onSlideEnd"
        >
          <!-- Slides with custom text -->
          <b-carousel-slide img-src="https://www.img.live/images/2018/06/18/ban1.jpg">
            <h1></h1>
          </b-carousel-slide>

          <b-carousel-slide img-src="https://www.img.live/images/2018/06/18/NoPath-Copy47.jpg">
            <h1></h1>
          </b-carousel-slide>
        </b-carousel>
      </div>
      <div class="col-md-4">
        <side-banner :imgSrc="imgUrl1" :title="title1"/>
        <side-banner :imgSrc="imgUrl2" :title="title2" class="img-w"/>
        <side-banner :imgSrc="imgUrl3" :title="title3" class="img-w"/>
      </div>
    </div>
  </div>
</template>

<script>
import SideBanner from './SideBanner'

export default {
  data () {
    return {
      slide: 0,
      sliding: null,
      imgUrl1: 'https://www.img.live/images/2018/06/18/NoPath-Copy10.jpg',
      imgUrl2: 'https://www.img.live/images/2018/06/18/mountain.jpg',
      imgUrl3: 'https://www.img.live/images/2018/06/18/NoPath-Copy46.jpg',
      title1: 'ทะเลและชายหาด',
      title2: 'ภูเขาและน้ำตก',
      title3: 'สถาปัตยกรรม'
    }
  },
  components: {
    'side-banner': SideBanner
  },
  methods: {
    onSlideStart (slide) {
      this.sliding = true
    },
    onSlideEnd (slide) {
      this.sliding = false
    }
  }
}
</script>
