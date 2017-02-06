<template>
<div id="partner" ref="partner">
  <div class="container">
    <h3>合作夥伴</h3>
    <div class="img-wrap">
      <img v-for="n in 3" :src="`/static/img/partner/partner-${n}.png`">
    </div>
  </div>
</div>

</template>

<script>
export default {
  name: 'Partner'
}
</script>

<style lang="sass" scoped>
$mblue: #1158A8
$mgreen: #65BDBC

#partner
  padding-top: 5%
  h3
    color: $mblue
  .img-wrap
    display: flex
    align-items: center
  img
    max-width: 31.333%
    padding: 0 1%

</style>