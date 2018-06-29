<template>
  <div>
    <Header />
    <Banner />
    <Money />
    <Footer />
    <Nav />
  </div>
</template>

<script>
import Header from '@/public/header'
import Banner from './banner'
import Footer from '@/public/footer'
import Nav from '@/public/nav'
import Money from '@/home/money'
export default {
  components: {
    Header,
    Banner,
    Footer,
    Money,
    Nav
  }
}
</script>

<style>

</style>
