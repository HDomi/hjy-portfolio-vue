<script setup lang="ts">
  import Maintit from '../components/MainTitle.vue'
  import DnItem from '../components/CardItem.vue'
</script>
<template>
    <div class="design">
      <Maintit maintit="퍼블리싱 관련 디자인을 Figma로 확인해보세요."/>
      <div class="ms_container">
        <a href="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2FozJKwbiSo5dToWKcppZMCd%2F%25ED%258E%25B8%25EC%259D%2598" target="_blank">
          <DnItem 
            dn_tit="감각있는 한지 쇼핑몰, 편의"
            dn_txt="화려한 색감을 표현하기 좋은 한지를 아이템으로 한 쇼핑몰을 만들어 보고 싶었습니다."
            dn_percent="100%"
            dn_sub="처음 작업물인 만큼 전체적인 디자인을 포토샵으로 작업 후에 그대로 만들어 내는 방법을 사용하였습니다."
          />
        </a>
        <a href="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2F7onpJ9jwufiW0BJtwWtXor%2F%25EB%258F%2584%25EB%25AF%25B8%25EB%2584%258C%25EC%258A%25A4" target="_blank">
          <DnItem 
            dn_tit="스마트한 컴퓨터 쇼핑몰, 도미넌스"
            dn_txt="컴퓨터를 판매하는 쇼핑몰을 만들어 보았습니다."
            dn_percent="100%"
            dn_sub="처음 작업물인 만큼 전체적인 디자인을 포토샵으로 작업 후에 그대로 만들어 내는 방법을 사용하였습니다."
          />
        </a>
        <a href="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2FHU7TI8ByPG5tFXzi0693cR%2F%25EC%258A%25A4%25EB%25A7%2588%25ED%258A%25B8%25EC%259E%25A5%25EB%25B6%2580_%25ED%2599%25A9%25EC%259E%25AC%25EC%2598%2581" target="_blank">
          <DnItem 
            dn_tit="스마트 패턴장부"
            dn_txt="기존 런칭중이던 스마트 패턴장부에 3개 페이지와 팝업창을 추가 하는 작업입니다."
            dn_percent="100%"
            dn_sub="figma를 사용하여 첫번째 디자인을 하였습니다. 처음 사용하는 툴인만큼 시행착오는 있었지만, 금방 적응하여 빠른 작업을 할 수 있었습니다."
          />
        </a>
        <a href="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2FveX6pqsXFSinb46vasr3RU%2F%25EC%258A%25A4%25EB%25A7%2588%25ED%258A%25B8%25EC%258B%259C%25ED%258B%25B0-%25ED%2591%259C%25EC%25A4%2580-%25EB%259D%25BC%25EC%259D%25B4%25EB%25B8%258C%25EB%259F%25AC%25EB%25A6%25AC-%25EC%25B5%259C%25EC%25A2%2585" target="_blank">
          <DnItem 
            dn_tit="스마트시티 라이브러리"
            dn_txt="정부지원 사업으로 진행되었던 프로젝트"
            dn_percent="100%"
            dn_sub="전체적인 디자인을 figma를 통해 작업하고, 클라이언트 측과 계속 소통해가며 더 나은 작업물을 위해 노력하였습니다."
          />
        </a>
        <a href="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2FbNU6UMwSDL9LPfXeTKdnEw%2F%25ED%258C%25A8%25ED%2584%25B4%25ED%2585%258C%25ED%2581%25AC-%25EB%258D%25B0%25EC%259D%25B4%25ED%2584%25B0%25EA%25B0%2580%25EA%25B3%25B5" target="_blank">
          <DnItem 
            dn_tit="데이터가공 서비스"
            dn_txt="이미지를 사이트 내에서 AI학습을 위한 형태로 쉽게 가공해주는 사이트입니다."
            dn_percent="100%"
            dn_sub="figma를 통한 작업이 어느정도 숙달되었기 때문에, 어렵지 않게 디자인 할 수 있었습니다."
          />
        </a>
        <a href="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2FdwJcOkbVxk5F0HqIv46HxW%2FDomi_Page" target="_blank">
          <DnItem 
            dn_tit="황재영의 포트폴리오 with React"
            dn_txt="황재영의 포트폴리오 입니다. 첫 React 작업물"
            dn_percent="100%"
            dn_sub="반복되는 페이지 layout이 많아, 전체적인 틀을 잡고 컨텐츠를 채워나가는 식으로 작업하였습니다."
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
    margin-bottom: 70px;
    display: flex;
    flex-direction: column;
    padding-top: 100px;
  }
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
  