<script setup lang="ts">
  import Maintit from '../components/MainTitle.vue'
  import DnItem from '../components/DesignItem.vue'
</script>
<template>
    <div class="design">
      <Maintit maintit="퍼블리싱 관련 디자인을 Figma로 확인해보세요."/>
      <div class="ms_container">
        <a href="">
          <DnItem 
            dn_tit="감각있는 한지 쇼핑몰, 편의"
            dn_txt="bb"
            dn_percent="100%"
          />
        </a>
        <a href="">
          <DnItem 
            dn_tit="스마트한 컴퓨터 쇼핑몰, 도미넌스"
            dn_txt="dd"
            dn_percent="100%"
          />
        </a>
        <a href="">
          <DnItem 
            dn_tit="스마트 패턴장부"
            dn_txt="dd"
            dn_percent="100%"
          />
        </a>
        <a href="">
          <DnItem 
            dn_tit="스마트시티 라이브러리"
            dn_txt="dd"
            dn_percent="100%"
          />
        </a>
        <a href="">
          <DnItem 
            dn_tit="데이터가공 서비스"
            dn_txt="dd"
            dn_percent="100%"
          />
        </a>
      </div>
    </div>
  </template>
  
  <style>
.ms_container{
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    z-index: 1;
}
.design {
    display: flex;
    flex-direction: column;
    padding-top: 80px;
  }
  .design{padding-top: 100px;}
  @media (min-width: 1024px) {
    .design {
      min-height: 100vh;
      display: flex;
      align-items: center;
    }
    .ms_container{
    display: grid;
    grid-template-columns: auto auto;
  }
  }
  </style>
  