<template>
<div>
    <Swiper :items="items" :class="$style.m20" />
</div>
</template>

<script>
import Swiper from '@/common/swiper'
export default {
  components: {
    Swiper
  },
  data: function () {
    return {
      items: [
        {
          src: '//img12.360buyimg.com/jrpmobile/jfs/t20827/298/1700997090/51227/3b3da20b/5b3225f6N9ca7cafd.jpg?width=750&height=320',
          href: '#'
        }, {
          src: '//img12.360buyimg.com/jrpmobile/jfs/t20827/298/1700997090/51227/3b3da20b/5b3225f6N9ca7cafd.jpg?width=750&height=320',
          href: '#'
        }
      ]
    }
  }
}
</script>

<style module>
.m20{
  margin-top: 20px;
}
</style>
