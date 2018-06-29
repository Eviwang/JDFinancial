<template>
  <footer>
    <img src="//img12.360buyimg.com/jrpmobile/jfs/t2842/350/3035567089/14791/5f6ff93d/577cf395N31e76288.png?width=1125&height=252"/>
    <dl>
      <dt>
        <div class="item">
          <img src="http://img12.360buyimg.com/jrpmobile/jfs/t2971/333/1297567079/898/f2d2e00d/577dc28dNe5138337.png?width=108&height=108" alt="">
          <p>客户端</p>
        </div>
        <div class="item">
          <img src="http://img12.360buyimg.com/jrpmobile/jfs/t2971/333/1297567079/898/f2d2e00d/577dc28dNe5138337.png?width=108&height=108" alt="">
          <p>客户端</p>
        </div>
        <div class="item">
          <img src="http://img12.360buyimg.com/jrpmobile/jfs/t2971/333/1297567079/898/f2d2e00d/577dc28dNe5138337.png?width=108&height=108" alt="">
          <p>客户端</p>
        </div>
      </dt>
      <dd>
        Copyright © 2004-2018 京东JD.com 版权所有
      </dd>
      <dd>
        投资有风险，购买需谨慎
      </dd>
      <dd>
        京东金融平台服务协议
      </dd>
      <dd>
        京东金融隐私政策
      </dd>
    </dl>
  </footer>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
  footer{
    color:#999;
    margin-top:20px;
    margin-bottom:20px;
    img{
        height: 144px;
        width: 100%;
    }
    dt{
        display: flex;
        justify-content: space-around;
        padding-top: 40px;
        padding-bottom:20px;
        .item{
          width:33.3333%;
          text-align: center;
          font-size: 26px;
          img{
            width:90px;
            height: 90px;
          }
        }
    }

  }
  dd:nth-of-type(n+1){
      font-size: 24px;
      line-height: 1.6;
      padding: 24px 32px;
      text-align: center;
    }
  dt,dd:not(:last-child){
    border-bottom: solid 1px #DDD;
  }
</style>
