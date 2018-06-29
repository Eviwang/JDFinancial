<template>
  <div :class="['panel',className]">
    <h4>-{{title}}- <span v-if="subTitle">{{subTitle}}</span></h4>
    <slot />
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: ''
    },
    subTitle: {
      type: String,
      default: ''
    },
    className: {
      type: String,
      default: ''
    }
  }
}
</script>

<style lang="scss" scoped>
@import '@/css/common.scss';
.panel{
  background:#fff;
  >h4{
    line-height: 112px;
    text-align: center;
    color:#333;
    font-weight: 700;
    font-size: 32px;
    position: relative;
    span{
      position: absolute;
      right:32px;
      font-size: 28px;
      font-weight: normal;
      @include middle();
      color:#999;
      background:url("//m.jr.jd.com/spe/qyy/main/images/icon_arrow1.png") center right no-repeat;
      background-size: 18px 24px;
      padding:0 32px;
    }
  }
}
</style>
