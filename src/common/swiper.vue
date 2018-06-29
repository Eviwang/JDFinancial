<template>
 <swiper ref="mySwiper" :options="options" :class="['banner',className]">
    <!-- slides -->
    <swiper-slide v-for="item of items" :key="item.url">
      <a :href="item.href">
        <img :src="item.src"/>
      </a>
    </swiper-slide>
    <!-- Optional controls -->
    <div class="swiper-pagination" slot="pagination"></div>
  </swiper>
</template>

<script>
import 'swiper/dist/css/swiper.css'
import { swiper, swiperSlide } from 'vue-awesome-swiper'
export default {
  components: {
    swiper,
    swiperSlide
  },
  props: {
    className: {
      type: String,
      default: ''
    },
    items: {
      type: Array,
      default: () => []
    },
    swiperOption: {
      type: Object,
      default: () => ({})
    }
  },
  data: () => {
    let defaultOptions = {
      autoplay: {
        disableOnInteraction: false
      },
      pagination: {
        el: '.swiper-pagination',
        clickable: true
      }
    }
    return {
      options: Object.assign(defaultOptions, this.swiperOption)
    }
  }

}
</script>

<style lang="scss" scoped>
   .banner{
     height: 272px;
   }
   .swiper-slide{
    img{
      width: 100%;
      height: 100%;
    }
   }
</style>
