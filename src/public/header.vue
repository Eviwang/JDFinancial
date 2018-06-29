<template>
  <div class="header">
    <div class="login">
      <a>注册</a>&nbsp;|&nbsp;<a>登录</a>
    </div>
    <img src="//m.jr.jd.com/spe/qyy/main/images/jr-logo.png" class="logo" />
    <button>
      APP下载
    </button>
  </div>
</template>

<script>
export default {
  components: {

  },
  data: () => {
    return {

    }
  }
}
</script>

<style lang="scss" scoped>
@import '../css/common.scss';
.header{
  position: fixed;
  left: 0;
  right: 0;
  top:0;
  height: 100px;
  z-index: 999;
  text-align:center;
  background:#fff;
  .logo{
    display: block;
    margin: 18px auto;
    height: 56px;;
  }
  .login{
    left: 36px;
    line-height: 30px;
    color:#666;
    @include middle();
  }
  button{
    font-size: 28px;
    line-height: 56px;
    right: 24px;
    font-weight: 400;
    @include btn();
    @include middle();
  }
}

</style>
