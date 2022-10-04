<script setup lang="ts">
    defineProps<{
        dn_tit: string,
        dn_txt: string,
        dn_percent: any,
        dn_sub: string
    }>()
</script>
<template>
    <div class="p_card">
        <div class="p_content">
            <h3>{{ dn_tit }}</h3>
            <p>{{ dn_txt }}<br/>기여도 : {{ dn_percent }}</p>
            <div class="click_txt">Hover & Click</div><br/>
            <div class="p_card_sub">디자인에 대해..<br/><span><br/>{{ dn_sub }}</span></div>
        </div>
    </div>
</template>
<style scoped>
.p_card:hover .p_card_sub{
    display: block;
    transition: .45s;
}
.p_card_sub span{
    font-weight: normal;
}
.p_card_sub{
    font-weight: bold;
    display: none;
    transition: .45s;
}
.p_card:hover{
    height: 400px;
    transition: .45s;
}
.p_card{
    padding: 20px;
    position: relative;
    width: 260px;
    transition: .45s;
    height: 220px;
    margin: 15px;
    box-shadow: 20px 20px 50px rgba(0,0,0,0.5);
    border-radius: 15px;
    background: rgba(255, 255, 255, 0.1);
    overflow: hidden;
    display: flex;
    justify-content: center;
    align-items: center;
    border-top: 1px solid rgba(255, 255, 255, 0.5);
    border-left: 1px solid rgba(255, 255, 255, 0.5);
    backdrop-filter: blur(5px);
}
.click_txt{
    color: hsla(160, 100%, 37%, 1);
    font-size: 0.9em;
    position: absolute;
    right: -6px;
    bottom: -10px;
}
.p_content{
    position: relative;
    width: 100%;
    height: 100%;
}
.p_content h3{
    color: hsla(160, 100%, 37%, 1);
    font-size: 1.2em;
    text-align: left;
    color: #fff;
}
.p_content p{
    text-align: left;
    font-size: 1em;
    margin-top: 10px;
    color: #fff;
    font-weight: 300;
}
@media (max-width: 1024px) {
.p_card_sub{
    display: block !important;;
    transition: .45s;
}
.p_card_sub{
    font-weight: bold;
    display: none;
    transition: .45s;
}
.p_card{
    height: 400px;
    transition: .45s;
}
}
</style>