<template>
    <ul :class="['menu',className]">
      <li v-for="item of menus" :key="item.href">
        <router-link :to="{path:item.href}">
          <i :class="item.icon"></i>
          {{item.text}}
        </router-link>
      </li>
    </ul>
</template>

<script>
export default {
  props: {
    menus: {
      type: Array,
      default: () => []
    },
    className: {
      type: String,
      default: ''
    }
  },
  mounted: () => {
    console.log(this.className)
  }
}
</script>

<style lang="scss" scoped>
@import '@/css/common.scss';
.menu{
    display: flex;
    justify-content: center;
    li{
      color: #B1B4BB;
      display: block;
      i{
        display: block;
        font-size: 40px;
        line-height: 44px;
        height: 44px;
      }
      a{
         padding-top:20px;
         height: 500%;
         width: 100%;
         display: block;
      }
      .router-link-active{
          color:#4668FF;
      }
    }
  }

</style>
