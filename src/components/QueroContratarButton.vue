<script setup>
import WhatsAppIcon from './icons/WhatsAppIcon.vue'

function openWhatsapp(){
    window.open('https://api.whatsapp.com/send?phone=5541987517945&text=Ol%C3%A1,%20vim%20pelo%20site%20e%20gostaria%20de%20um%20atendimento!','_blank')
}
</script>

<template>
    <div @click="openWhatsapp">
        <span>Quero contratar!</span>
        <WhatsAppIcon class="icon"/>
    </div>
</template>

<style scoped>
div{
    height: fit-content;
    padding: 20px 50px;

    font-size: 20px;
    font-weight: 500;
    text-shadow: 0px 0px 0px rgba(0, 0, 0, 0);
    fill: #fff;
    color: #fff;
    background-color: transparent;
    background-image: linear-gradient(180deg, #23b14d 0%, #3cdb42 100%);
    border-radius: 500px;
    box-shadow: 0px 0px 20px 0px rgba(0, 255, 12.195652173913029, .38);
    padding: 20px 50px;
    width: fit-content;

    display: flex;
    align-items: center;
    transition: .3s ease-out;

    cursor: pointer;
}
div:hover{
    transform: translate(0px, -8px);
}
.icon{
    height: 24px;
    margin-left: 6px;
}
</style>