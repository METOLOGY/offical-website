<template>
<div id="records" ref="records">
  <div class="container">
    <h3>參賽與獲獎紀錄</h3>
    <div class="row">
      <div class="four columns record" >
        <div class="record-img-wrap" v-for="n in 3">
          <img :src="`/static/img/records/record-${n}.jpg`">
          <p>{{ imgDesc[n] }}</p>
        </div>
      </div>
      <div class="four columns record">
        <div class="record-img-wrap" v-for="n in 3">
          <img :src="`/static/img/records/record-${n+3}.jpg`">
           <p>{{ imgDesc[n+3] }}</p>
        </div>
      </div>
      <div class="four columns record">
        <div class="record-img-wrap" v-for="n in 2" >
          <img :src="`/static/img/records/record-${n+6}.jpg`">
           <p>{{ imgDesc[n+6] }}</p>
        </div>
      </div>
    </div>
  </div>
</div>



</template>

<script type="text/javascript">
export default {
  name: 'Records',
  data () {
    return {
      imgDesc: [
        '',
        '台大創創挑戰賽 複賽',
        '中國創新創業大賽 決賽',
        'H.Spectrum',
        '30青創實驗室 銀牌',
        'Trans論壇',
        'Startup World Cup WarmUp 評審獎第二名',
        '上海海峽兩岸創業競賽 三等獎',
        '廣東中山青年創業大賽 複賽'
      ]
    }
  }
}
</script>

<style lang="sass" scoped>
$mblue: #1158A8
$mgreen: #65BDBC

#records
  padding-top: 10%
  h3
    text-align: right
    color: $mblue

.record
  text-align: center
  .record-img-wrap
    padding-bottom: 2%
  img
    border-radius: 10px
    width: 100%

</style>
