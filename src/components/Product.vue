<template>
<!-- products -->
  <div id="products">
    <div class="product" id="debby"></div>
    <div class="product" id="HdataPred"></div>
    <div id="debby-mock-up">
      <img src="/static/img/mock-up.png">
      <video width="263" height="468" autoplay>
        <source src="/static/video/mock-up.mp4" type="video/mp4">
      </video>
    </div>

    <div class="" id="product-intro">
      <div class="container">
        <div class="row" id="debby-desc">
          <div class="one-half column">
            <h3>Debby - Line聊天機器人</h3>
            <p>記錄血糖、飲食紀錄，不再是容易忘記且麻煩的事情。Debby 在三餐飯後主動詢問您的飲食與血糖血糖狀況，並將所有資訊同步於雲端管理系統，隨時掌握過去數值，同時也是您任何關於糖尿病問題的小幫手。</p>
            <div class="qr-code">
              <img src="/static/img/qr.png">
            </div>
          </div>
          <div class="one-half column" id="debby-mock-up">
          </div>
        </div>

        <div class="row" id="HdataPred-desc">
          <div class="one-half column">
            <h3>HDataPred - 糖尿病風險預測</h3>
            <p>記錄血糖、飲食紀錄，不再是容易忘記且麻煩的事情。Debby 在三餐飯後主動詢問您的飲食與血糖血糖狀況，並將所有資訊同步於雲端管理系統，隨時掌握過去數值，同時也是您任何關於糖尿病問題的小幫手。</p>
            <button id="HdataPred-button">→ 免費預測</button>
          </div>
          <div class="one-half column" id="">
            <div class="button-middle">
              
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script type="text/javascript">
export default {
  name: 'Product'
}
</script>

<style lang="sass" scoped>
$mblue: #1158A8
$mgreen: #65BDBC

.product
  height: 60vh
  transform: rotate(-3deg);
  width: 104vw
  margin: -2vw

#products
  position: relative

#debby
  background-color: $mblue

#HdataPred
  background-color: $mgreen
  margin-top: 2%

#product-intro
  width: 100%
  position: absolute
  top: 10%
  z-index: 3
  color: white
  font-weight: 100
  p
    font-size: 18px

.qr-code
  img
    border-radius: 10px

#debby-mock-up
  position: absolute
  top: 10%;
  left: 65vw;
  img
    width: 250px
  video
    position: absolute;
    top: 16px;
    left: 12px;
    width: 224px;

#HdataPred-button
  min-width: 250px
  border-color: white
  color: white

#HdataPred-desc
  padding-top: 4em
  display: flex
</style>