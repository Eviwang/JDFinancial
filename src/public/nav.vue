<template>
  <Menu :menus="menus" :class-name="$style.menu2"></Menu>
</template>

<script>
import Menu from '@/common/menu'
export default {
  components: {
    Menu
  },
  data: () => {
    return {
      menus: [
        {
          text: '首页',
          src: 'https://img12.360buyimg.com/jrpmobile/jfs/t17650/174/1729132233/4020/2b09fc25/5ad6aac4N620fbed1.png?width=60&height=60',
          href: '/home',
          icon: 'icon-home3'
        },
        {
          text: '赚钱',
          src: 'https://img12.360buyimg.com/jrpmobile/jfs/t17650/174/1729132233/4020/2b09fc25/5ad6aac4N620fbed1.png?width=60&height=60',
          href: '/zhuanqian',
          icon: 'icon-coin-dollar'
        },
        {
          text: '借钱',
          src: 'https://img12.360buyimg.com/jrpmobile/jfs/t17650/174/1729132233/4020/2b09fc25/5ad6aac4N620fbed1.png?width=60&height=60',
          href: 'jieqian',
          icon: 'icon-credit-card'
        }, {
          text: '省钱',
          src: 'https://img12.360buyimg.com/jrpmobile/jfs/t17650/174/1729132233/4020/2b09fc25/5ad6aac4N620fbed1.png?width=60&height=60',
          href: 'sheng',
          icon: 'icon-coin-yen'
        }, {
          text: '会员',
          src: 'https://img12.360buyimg.com/jrpmobile/jfs/t17650/174/1729132233/4020/2b09fc25/5ad6aac4N620fbed1.png?width=60&height=60',
          href: 'huiyuan',
          icon: 'icon-user-tie'
        }
      ]
    }
  }
}
</script>

<style lang="scss" module>
.menu2{
  position: fixed;
  bottom: 0;
  left:0;
  right: 0;
  height: 100px;
  font-size: 22px;
  line-height: 32px;
  font-weight: 400;
  text-align: center;
  background:#f3f5f7;
  li{
    width: 20%;
    height: 100px;
    text-align: center;
    img{
      height: 44px;
      width: 44px;
      display: block;
      margin: 12px auto 6px auto;
    }
  }
}
</style>
