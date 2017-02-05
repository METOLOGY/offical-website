<template>
<div id="member">
  <div class="container">
    <h3>關於我們</h3>
  </div>
  <div class="member" v-for="item in member">
    <div class="container">
      <div class="row">
        <div class="two columns">
          <img :src="`/static/img/member/${item.img}`">
        </div>
        <div class="three columns">
          <h4>{{ item.name }}</h4>
        </div>
        <div class="seven columns">
          <p>{{ item.desc }}</p>
        </div>
      </div>
    </div>
  </div>

</div>

</template>

<script>
export default {
  name: 'Member',
  data () {
    return {
      member: [
        {
          name: '李承和',
          img: 'jason.png',
          desc: '富有理想，善於規劃事務與安排細節，確保團隊持續前進的重要推手，同時亦是團隊中核心般的存在。'
        },
        {
          name: '傅裕翔',
          img: 'edward.png',
          desc: '為人熱情，喜愛結交新朋友。覺得醫師不能只被動治療病患更該主動出擊， 口袋裡總是有許多 idea 可以拿出來討論。'
        },
        {
          name: '王偉安',
          img: 'weian.jpg',
          desc: '一位熱愛爬山、釣魚、羽球的工程師，豐富的生活之餘同時也相當專精於基因數據研究; 多年的研究與現今的工作實務經驗對於團隊的方向起了相當大的幫助。'
        },
        {
          name: '陳柏翰',
          img: 'pohan.jpg',
          desc: '對於科技愛不釋手，醫學影像也是。研究所期間持續鑽研電腦斷層影像演算法，希望可以將醫學影像診斷系統的力量帶進醫學界，為醫療界貢獻自己的小小心力！'
        },
        {
          name: '葉哲暠',
          img: 'howard.jpg',
          desc: '喜歡觀察日常生活周遭的人事物，並把為什麼套入在所觀察的事情裡。對人的行為和互動非常感興趣，因而自學使用者經驗設計，透過觀察和分析找出潛藏的關係和在渾沌中釐清要點。'
        },
        {
          name: '李哲銓',
          img: 'frank.jpg',
          desc: '樂於追求新知，有著工程人相當優異的整理歸納能力。在百般忙碌的課程、研究之餘，投入醫療資訊領域，結合自身資訊工程長才將團隊的紙上討論化為真實產品實現。'
        },
        {
          name: '李嘉軒',
          img: 'kelly.png',
          desc: '樂於體驗不同的事物，善於廣交朋友充實自我視野。擁有金融背景的專業，表達財務數據卻能淺顯意賅呈現。'
        },
        {
          name: '陳婉宜',
          img: 'nina.jpg',
          desc: '扎實的過每一天是她的原則，喜歡運用生物概念結合工程的方法進行有趣的研究。希望能將自己所學所能，連結各式領域的專業，將學界的精華帶入業界合作。'
        },
        {
          name: '馬聖翔',
          img: 'shan.png',
          desc: '把醫學的熱情透過筆記不斷的進行修煉，對於事物總有獨特的見解。同時經營被醫學同學譽為國考殺手的TINY Note醫學筆記網站。'
        }
      ]
    }
  }
}
</script>

<style lang="sass" scoped>
$mblue: #1158A8
$mgreen: #65BDBC

#member
  padding-top: 10%
  h3
    text-align: right
    color: $mblue
    padding-bottom: 3%

.member
  background-color: white
  width: 104vw
  margin: 0 -2vw
  maring-top: 1%
  transform: rotate(-3deg)
  .three
    text-align: center
    h4
      width: 100%
  h4, p
    margin: 0
    color: black
  &:nth-child(3n-1)
    background-color: $mblue
    h4, p
      color: white
  &:nth-child(3n)
    background-color: $mgreen
    h4, p
      color: white
  img
    width: 80%
    border-radius: 100%
  .row
    display: flex
    padding: 1% 0
    .columns
      display: flex
      align-items: center

</style>