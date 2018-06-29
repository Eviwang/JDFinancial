<template>
  <Panel title="理财精选" sub-title="更多">
    <ul class="content">
      <li v-for="i in 4" :key="i">
        <h4>
          京渤随享盈<span>理财推荐</span>
        </h4>
        <p class="rate">5.50%</p>
        <p class="history">历史年化收益率</p>
      </li>
    </ul>
  </Panel>
</template>

<script>
import Panel from '@/common/panel'
export default {
  components: {
    Panel
  }
}
</script>

<style lang="scss" scoped>
@import '@/css/common.scss';
  .content{
    display: flex;
    flex-wrap: wrap;
    li{
      position: relative;
      &:nth-child(2n+1)::after{
        width:1px;
        background:#eee;
        position: absolute;
        top:50%;
        right: 0;
        content: '';
        transform: translateY(-50%);
        height: 136px;
        display: block;
      }
      &:nth-child(n+3){
        border-top: 1px solid #eee;
      }
      width: 50%;
      padding-left: 32px;
      height: 218px;
       h4{
        line-height: 42px;
        font-size: 30px;
        margin:34px 0 16px;
        span{
            line-height: 34px;
            font-size: 22px;
            padding: 0 8px;
            color: #FF5155;
            border:1px solid #FF5155;
            margin-left: 8px;
        }
      }
      .rate{
          font-weight: 700;
          font-size: 44px;
          height: 58px;
          line-height: 58px;
          color: #FF5155;
          @include text-overflow-dot();
      }
      .history{
          font-size: 24px;
          height: 34px;
          line-height: 34px;
          color: #999;
          @include text-overflow-dot();
      }

    }
  }
</style>
