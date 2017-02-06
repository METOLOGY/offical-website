<template>
<div id="foot-nav" ref="foot-nav">
  <div class="container">
    <div class="row">
      <div class="three columns">
        <img src="/static/img/metology-icon-white.png">
      </div>
      <div class="nine columns">
        <div class="nav">
          <ul class="navbar">
            <li @click="toProduct">產品</li>
            <li @click="toMember">關於我們</li>
            <li><a href="mailto:metology.taiwan@gmail.com">聯繫我們</a></li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: 'FootNav',
  methods: {
    toProduct () {
      const currentPosition = document.documentElement.scrollTop || document.body.scrollTop
      const productPosition = this.$parent.$refs.product.$el.offsetTop
      // console.log(currentPosition, productPosition)
      scrollAnimate(currentPosition, productPosition)
    },
    toMember () {
      // console.log('to member')
      const currentPosition = document.documentElement.scrollTop || document.body.scrollTop
      const memberPosition = this.$parent.$refs.member.$el.offsetTop
      // console.log(currentPosition, memberPosition)
      scrollAnimate(currentPosition, memberPosition)
    }
  }
}

function scrollAnimate (current, target) {
  for (let i = current; i > target; i--) {
    console.log(i)
    setTimeout(() => { window.scrollTo(0, i) }, 0 + (0.3 * i))
    // if (i === 1) console.log(i)
  }
}

</script>

<style lang="sass" scoped>
$mblue: #1158A8
$mgreen: #65BDBC

#foot-nav
  margin-top: 5%
  padding: 2% 0
  background-color: $mblue
  .row
    display: flex
  img
    width: 100px
  li
    color: white
    font-size: 16px
    cursor: pointer;
  a
    color: white
    text-decoration: none

</style>