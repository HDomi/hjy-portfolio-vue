<script setup lang="ts">
  import Maintit from '../components/MainTitle.vue'
  import DnItem from '../components/CardItemDev.vue'
</script>
<template>
    <div class="portfolio">
      <Maintit maintit="퍼블리싱/FE 작업물들을 확인해보세요."/>
      <div class="ms_container">
        <a href="https://hwang1139.cafe24.com/html/pnei/main.html" target="_blank">
          <DnItem 
            dn_tit="감각있는 한지 쇼핑몰, 편의"
            dn_txt="html,css를 사용, 기본적인 동작을을 javascript로 구현하였습니다."
            dn_percent="100%"
            dn_sub="처음하는 작업이었으나, 수많은 구글링을 통해 완성하였습니다. 이는 나중에 비슷한 작업이 이루어 질 때 큰 도움을 주었습니다."
          />
        </a>
        <a href="https://hwang1139.cafe24.com/html/dominc/main.html" target="_blank">
          <DnItem 
            dn_tit="스마트한 컴퓨터 쇼핑몰, 도미넌스"
            dn_txt="html,css를 사용, 기본적인 동작을을 javascript로 구현하였습니다."
            dn_percent="100%"
            dn_sub="처음하는 작업이었으나, 수많은 구글링을 통해 완성하였습니다. 이는 나중에 비슷한 작업이 이루어 질 때 큰 도움을 주었습니다."
          />
        </a>
        <a href="https://hdomi.github.io/smartpr/views/login.html" target="_blank">
          <DnItem 
            dn_tit="스마트 패턴장부"
            dn_txt="기존 런칭중이던 WebApp에 페이지를 추가하는 형태라 기존 사용중이던 padding, margin값 등을 참고하여 개발하였습니다."
            dn_percent="100%"
            dn_sub="시간 설정을 넣거나, 토글버튼 등 여러 라이브러리와 예제를 참고하여 완성하였습니다. 이는 이후 작업에도 큰 도움을 주었습니다."
          />
        </a>
        <a href="https://hdomi.github.io/smartcity/views/main" target="_blank">
          <DnItem 
            dn_tit="스마트시티 라이브러리"
            dn_txt="기본적인 작업 이외에도 반응형을 구현하기 위해 미디어쿼리 등을 사용하여 반응형 작업을 했습니다."
            dn_percent="100%"
            dn_sub="레이아웃을 계속 살펴가며 반응형의 완성도에 중점을 두었습니다."
          />
        </a>
        <a href="https://hdomi.github.io/datacorp/views/main" target="_blank">
          <DnItem 
            dn_tit="데이터가공 서비스"
            dn_txt="미디어쿼리 등을 사용하였으며, 레이아웃이 그대로 유지되어야 하는 페이지는 javascript를 통해 구현하였습니다."
            dn_percent="100%"
            dn_sub="figma를 통한 작업이 어느정도 숙달되었기 때문에, 어렵지 않게 디자인 할 수 있었습니다."
          />
        </a>
        <a href="https://hdomi.github.io/portfolio/" target="_blank">
          <DnItem 
            dn_tit="황재영의 포트폴리오 with React"
            dn_txt="React의 전반적인 구조 파악 및 반응형 작업에 초점을 두었습니다."
            dn_percent="100%"
            dn_sub="React를 사용한 첫번째 작업물이며, 컴포넌트, react hook등을 분리하여 컴포넌트 재사용에 초점을 두었습니다."
          />
        </a>
      </div>
    </div>
  </template>
  
  <style>
    .portfolio {
      min-height: 100vh;
      display: flex;
      align-items: center;
      flex-direction: column;
      padding-top: 100px;
      margin-bottom: 60px;
    }
    .ms_container{
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    z-index: 1;
}
  @media (min-width: 1024px) {
    .ms_container{
    display: grid;
    grid-template-columns: auto auto;
  }
  }
  </style>
  