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
          <li>產品</li>
          <li>關於我們</li>
          <li>聯繫我們</li>
        </ul>
      </div>
    </div>
  </div>
</div>

</template>

<script>
export default {
  name: 'Navbar'
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
</style>