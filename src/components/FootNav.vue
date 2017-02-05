<template>
<div id="foor-nav">
  <div class="container">
    <div class="row">
      <div class="three columns">
        <img src="/static/img/metology-icon-white.png">
      </div>
      <div class="nine columns">
        <div class="nav">
          <ul class="navbar">
            <li>產品</li>
            <li>關於我們</li>
            <li>聯繫我們</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
</div>
</template>

<script>
export default {
  name: 'FootNav'
}
</script>

<style lang="sass" scoped="">
$mblue: #1158A8
$mgreen: #65BDBC

#foor-nav
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
</style>