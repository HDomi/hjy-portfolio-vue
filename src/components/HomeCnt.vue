<script setup lang="ts">
import HomeItem from './HomeItem.vue'


import HeartIcon from './icons/IconHeart.vue'
import IconCube from './icons/IconCube.vue'
import ToolingIcon from './icons/IconTooling.vue'

</script>
<template>
  <HomeItem>
    <template #icon>
      <HeartIcon />
    </template>
    <template #heading>슬로건</template>
      기업의 이익과 동시에 자신의 능력 향상을 추구합니다.
  </HomeItem>

  <HomeItem>
    <template #icon>
      <IconCube />
    </template>
    <template #heading>기술스택</template>
      <div class="stack_wrap">
        <div class="stack_cnt">
          <img alt="HTML5" src="@/assets//main_ic/ic_html5.png" width="30"/>
          &nbsp;HTML5
        </div>
        <div class="stack_cnt">
          <img alt="CSS3" src="@/assets//main_ic/ic_css3.png" width="30"/>
          &nbsp;CSS3
        </div>
        <div class="stack_cnt">
          <img alt="Javascript" src="@/assets//main_ic/ic_js.png" width="30"/>
          &nbsp;Javascript
        </div>
        <div class="stack_cnt">
          <img alt="Vue" src="@/assets//main_ic/ic_vue.png" width="30"/>
          &nbsp;Vue
        </div>
        <div class="stack_cnt">
          <img alt="Ts" src="@/assets//main_ic/ic_ts.png" width="30"/>
          &nbsp;Ts
        </div>
      </div>
  </HomeItem>

  <HomeItem>
    <template #icon>
      <ToolingIcon />
    </template>
    <template #heading>간략 자기소개</template>
      안녕하세요. 황재영입니다.<br/>
      지난 1년간 웹디자인/퍼블리셔로 근무하다 본격적으로<br/>
      프론트엔드의 길로 가기 위해 공부중에 있습니다.<br/>
      HTML5와 CSS3, 간단한 Javascript등에는 자신이 있으나<br/>
      Vue, Ts부분은 아직 많이 미흡하고 부족합니다.<br/><br/>
      하지만 지금 이 페이지를 만드는 것 처럼<br/>꾸준히 노력하고 공부중입니다. 감사합니다.
  </HomeItem>
</template>


<style>
  .stack_wrap{
    display: flex;
  }
  .stack_cnt{
    margin-left: 15px;
    display: flex;
    justify-content: center;
    align-items: center;
  }
  .stack_cnt:first-of-type{margin-left: 0;}
</style>