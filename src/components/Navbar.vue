<template>

<!-- navbar -->
<div class="container" id="navbar">
  <div class="row">
    <div class="five columns">
      <h3>深入淺出您的健康指數， 讓Metology為您紀錄每個血糖細節。</h3>
    </div>
    <div class="seven columns">
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

</template>

<script>
export default {
  name: 'Navbar',
  methods: {
    toProduct () {
      const currentPosition = document.documentElement.scrollTop || document.body.scrollTop
      const productPosition = this.$parent.$refs.product.$el.offsetTop

      scrollAnimate(currentPosition, productPosition)
    },
    toMember () {
      const currentPosition = document.documentElement.scrollTop || document.body.scrollTop
      const memberPosition = this.$parent.$refs.member.$el.offsetTop

      scrollAnimate(currentPosition, memberPosition)
    }
  }
}

function scrollAnimate (current, target) {
  for (let i = current; i < target; i++) {
    setTimeout(() => { window.scrollTo(0, i) }, 1 + (0.3 * i))
  }
}

</script>

<style lang="sass">
$mblue: #1158A8
$mgreen: #65BDBC

#navbar
  padding: 5em 0
  .row
    display: flex

.nav
  float: right
  height: 100%
  display: flex
  align-items: center
  .navbar
    list-style: none
    display: flex
    margin: 0px
    li
      padding-left: 2em
      color: $mblue
      font-size: 20px
      cursor: pointer;
    a
      color: $mblue
      text-decoration: none
</style>