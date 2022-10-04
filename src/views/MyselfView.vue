<script setup lang="ts">
  import Card_tilt from '../components/Card_tilt.vue'
  import Subtit from '../components/SubTitle.vue'
  import BoxTxt from '../components/BoxTxt.vue'
</script>
<template>
  <div class="myself">
    <Subtit subtit="자격증"/>
    <div class="ex_card_wrap">
      <BoxTxt ex_name="웹디자인 기능사" />
      <BoxTxt ex_name="GTQ 포토샵 1급" />
      <BoxTxt ex_name="네트워크 관리사 2급" />
      <BoxTxt ex_name="컴퓨터활용능력 2급" />
      <BoxTxt ex_name="MOS PPT2016" />
    </div>
    <Subtit subtit="히스토리"/>
    <div class="ms_container">
      <Card_tilt 
      card_num="01" 
      card_tit="고등학교 재학 당시"
      card_txt="용인고등학교App 개발"
      card_date="June 2016."
      />
      <Card_tilt 
      card_num="02" 
      card_tit="국제대학교"
      card_txt="컴퓨터공학과 졸업"
      card_date="February 2021."
      />
      <Card_tilt 
      card_num="03" 
      card_tit="두드림 컴퓨터 아카데미"
      card_txt="웹디자이너 / 웹퍼블리셔 양성과정 교육 수료"
      card_date="August 2021."
      />
      <Card_tilt 
      card_num="04" 
      card_tit="닷네임코리아"
      card_txt="디자인팀 / 웹 유지보수 및 개발"
      card_date="Oct 2021 ~ing 2022."
      />
    </div>
  </div>
</template>

<style>
.ex_card_wrap{
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-bottom: 50px;
}
.ms_container{
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    z-index: 1;
}
.myself {
    padding-top: 80px;
    margin-bottom: 50px;
  }
@media (max-width: 1024px) {
  .ms_container{
    display: grid;
    grid-template-columns: auto auto;
  }
  .myself {
    min-height: 100vh;
  }
  .ex_card_wrap{
    display: grid;
    justify-content: space-around;
  }
}
@media (max-width: 690px) {
  .ms_container{
    display: grid;
    grid-template-columns: auto;
  }
}
</style>
