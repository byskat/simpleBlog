<template>
  <div class="bg-gray-200 font-sans leading-normal tracking-normal">
    <mainHeader></mainHeader>
    <!--Container-->
    <div class="container px-4 md:px-0 max-w-6xl mx-auto -mt-32">
      <nuxt />
      <cta></cta>
      <ctaAuthor></ctaAuthor>
    </div>
    <mainFooter></mainFooter>
  </div>
</template>

<script>
import animate from 'animate.css'
import MainHeader from '~/components/MainHeader.vue'
import Cta from '~/components/Cta.vue'
import CtaAuthor from '~/components/CtaAuthor.vue'
import MainFooter from '~/components/MainFooter.vue'

export default {
  name: 'mainView',
  components: {
    MainHeader,
    Cta,
    CtaAuthor,
    MainFooter
  }
}
</script>

<style>
html {
  font-family: 'Source Sans Pro', -apple-system, BlinkMacSystemFont, 'Segoe UI',
    Roboto, 'Helvetica Neue', Arial, sans-serif;
  font-size: 16px;
  word-spacing: 1px;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
  -moz-osx-font-smoothing: grayscale;
  -webkit-font-smoothing: antialiased;
  box-sizing: border-box;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

.smooth {
  transition: box-shadow 0.3s ease-in-out;
}

.button--green {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #3b8070;
  color: #3b8070;
  text-decoration: none;
  padding: 10px 30px;
}

.button--green:hover {
  color: #fff;
  background-color: #3b8070;
}

.button--grey {
  display: inline-block;
  border-radius: 4px;
  border: 1px solid #35495e;
  color: #35495e;
  text-decoration: none;
  padding: 10px 30px;
  margin-left: 15px;
}

.button--grey:hover {
  color: #fff;
  background-color: #35495e;
}
</style>
