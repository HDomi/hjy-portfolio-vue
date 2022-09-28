<script setup lang="ts">
    defineProps<{
        ex_name: string,
    }>()
</script>
<template>
    <div class="card">
        <div class="ro_box"></div>
        <div class="card_tit">{{ ex_name }}</div>
    </div>
</template>
<style scoped>
.card{
    display: flex;
    margin-top: 15px;
}
.card_tit{
    font-size: 1rem;
    font-weight: bold;
    color: #fff;
}
.ro_box {
    width: 15px;
    height: 15px;
    display: inline-block;
    background-color: hsla(160, 100%, 37%, 1);
    border: 1px solid #000;
    transition:0.15s ease-in;
    margin-right: 5px;
}
        
.ro_box:hover {
    width: 17px;
    height: 17px;
    background-color: hsla(160, 100%, 37%, 0.2);
    transform: rotate(45deg);
}
</style>