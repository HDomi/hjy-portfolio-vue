<script setup lang="ts">
  import Maintit from '../components/MainTitle.vue'

</script>
<template>
    <div class="contact">
      <Maintit maintit="이메일을 보내주세요!" />
      <div class="cntac_mail">
        <form ref="form">
          <ul>
            <li><input type="text" class="cntac_txtbar" placeholder="제목" name="user_title"/></li>
            <li><input type="text" class="cntac_txtbar" placeholder="전화번호 *선택사항*" name="user_phone"/></li>
            <li><input type="email" class="cntac_txtbar" placeholder="이메일" name="user_email"/></li>
            <li><textarea class="cntac_txtbar txtbar_rec" placeholder="내용" name="user_message"/></li>
            <button type="submit" class="cntac_btn" value="Send">보내기</button>
          </ul>
        </form>
      </div>
    </div>
  </template>
  
  <style>
.contact{
  display: flex;
  flex-direction: column;
  padding-top: 100px;
}
.cntac_mail *{
    color: #fff;
}
.cntac_mail ul{
  padding: 0;
}
.cntac_mail{
    display: block;
    width: 100%;
    border-radius:8px;
    margin-top: 30px;
    padding: 10px;
}
.cntac_txtbar{
    width: 100%;
    height: 40px;
    margin-bottom: 15px;
    padding-left: 10px;
    box-sizing: border-box;
    border-top: 1px solid rgba(255, 255, 255, 0.5);
    border-left: 1px solid rgba(255, 255, 255, 0.5);
    backdrop-filter: blur(5px);
    border-radius: 2px;
    background: rgba(255, 255, 255, 0.1);
}
.cntac_txtbar::placeholder{
    color: #fff;
}
.txtbar_rec{
    height: 300px;
}
.cntac_btn{
    border: 1px solid #161623;
    width: 100%;
    height: 40px;
    margin-top: 30px;
    box-sizing: border-box;
    color: #fff;
    border-top: 1px solid rgba(255, 255, 255, 0.5);
    border-left: 1px solid rgba(255, 255, 255, 0.5);
    backdrop-filter: blur(5px);
    border-radius: 15px;
    background: hsla(160, 97%, 39%, 0.542);border-radius:5px;
    margin-bottom: 100px;
    cursor: pointer;
    font-weight: 700;
}
.cntac_btn:hover{
    background: rgba(0, 189, 126, 0.815);
}
/*웹퍼블리싱*/
.webpub_sec{
    
    height: 100%;
    margin-bottom: 150px;
}
.cnt_inner_wrap3{
    width: 100%;
    height: 100%;
    display: grid;
    grid-template-columns: auto auto;
}
  @media (min-width: 1024px) {
    .contact {
      min-height: 100vh;
      display: flex;
      align-items: center;
    }
  }
  </style>
  