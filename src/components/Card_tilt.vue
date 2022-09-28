<script setup lang="ts">
    defineProps<{
        card_num: string,
        card_tit: string,
        card_txt: string,
        card_date: string
    }>()
</script>
<template>
    <div class="p_card">
        <h2>{{ card_num }}</h2>
        <div class="p_content">
            <h3>{{ card_tit }}</h3>
            <p>{{ card_txt }}</p>
        </div>
        <div class="p_card_btn">{{ card_date }}</div>
    </div>
</template>
<style scoped>
.p_card{
    padding: 20px;
    position: relative;
    width: 260px;
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
.p_content{
    position: relative;
    width: 100%;
    height: 100%;
}
.p_card h2{
    position: absolute;
    bottom: -60px;
    right: -20px;
    font-size: 130px;
    color: rgba(255, 255, 255, 0.05);
}
.p_content h3{
    font-size: 1.5em;
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
.p_card_btn{
    position: absolute;
    display: inline-block;
    padding: 5px;
    width: 200px;
    text-align: center;
    background: hsla(160, 100%, 37%, 1);
    color: #fff;
    border-radius: 20px;
    text-decoration: none;
    font-weight: 500;
    left: 50%;
    transform: translateX(-50%);
    bottom: 20px;
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.35);
}
</style>