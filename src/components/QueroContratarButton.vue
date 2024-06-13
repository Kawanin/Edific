<script setup>
import WhatsAppIcon from './icons/WhatsAppIcon.vue'
</script>

<template>
    <div>
        <a href="">
            <span>Quero contratar!</span>
            <WhatsAppIcon class="icon"/>
        </a>
    </div>
</template>

<style scoped>
a{
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
}
a:hover{
    transform: translate(0px, -8px);
}
.icon{
    height: 24px;
    margin-left: 6px;
}
</style>