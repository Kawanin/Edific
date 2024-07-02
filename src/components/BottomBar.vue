<template>
    <div class="wrapper">
        <div class="container">
            <div class="enterprise-logo">
                <img :src="enterpriseLogo" alt="">
            </div>
            <div class="social-network">
                <span>Nossas redes sociais:</span>
                <div>
                    <EmailIcon class="icon" />
                    <span>{{ email }}</span>
                </div>
                <div  @click="openInstagram">
                    <InstagramIcon class="icon" />
                    <span>{{ instagram }}</span>
                </div>
                <div  @click="openWhatsapp">
                    <WhatsAppIcon class="icon" />
                    <span>{{ whatsapp }}</span>
                </div>
            </div>
        </div>
        <div class="copyright-container">
            <p>Copyright 2023 © TAB Engenharia –  Todos os direitos reservados.</p>
        </div>
    </div>
</template>

<script setup>
import EmailIcon from './icons/EmailIcon.vue';
import InstagramIcon from './icons/InstagramIcon.vue';
import WhatsAppIcon from './icons/WhatsAppIcon.vue';

defineProps({
    enterpriseLogo: {
        type: String,
        required: true
    },
    email: {
        type: String,
        required: true
    },
    instagram: {
        type: String,
        required: true
    },
    whatsapp: {
        type: String,
        required: true
    },
})

function openWhatsapp(){
    window.open('http://google.com','_blank')
}
function openInstagram(){
    window.open('http://google.com','_blank')
}
</script>

<style scoped>
.wrapper{
    width: 100vw;
    height: 250px;
    background-color: #0D0703;
    color: #FFFFFF;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    position: relative;


    
    position: absolute;
    top: 0;
    left: 0;
}
.container {
    width: 1015px;
    height: 150px;
    display: flex;
    margin-bottom: 40px;
}

.container > div {
    flex-grow: 1;
    width: 50%;
}

.enterprise-logo{
    display: flex;
    justify-content: right;
    padding-right: 32px;
    align-items: center;
}

.enterprise-logo > img {
    max-width: 200px;
    height: fit-content;
}

.icon {
    height: 25px;
    width: fit-content;
    filter: brightness(100);
    fill: #FFFFFF;
    margin-right: 8px;
}

.social-network {
    display: flex;
    flex-direction: column;
    justify-content: center;
    border-left: 1px solid #FFFFFF;
    padding-left: 32px
}
.social-network > span{
   margin-bottom: 6px;
}

.social-network > div {
    height: 50px;
    width: 100%;
    display: flex;
    align-items: center;
}
.social-network > div:not(:first-child) {
    cursor: pointer;
}
.copyright-container{
   position: absolute;
   bottom: 0;
   padding: 20px;
}
@media (max-width: 760px) {
    .container{
        flex-direction: column;
        height: 350px;
        margin-bottom: 0px;
        width: 400px;
        position: relative;
        background-color: blue;
        justify-content: center;
        align-items: center;
    }
    .wrapper{
        height: 400px;
    }
    .social-network {
        border-left: none;
        background-color: red;
        padding-left: 0;
        width: 10px;
    }
    .enterprise-logo{
        display: flex;
        justify-content: center;
        align-items: center;
        padding-right: 0;
        background-color: brown;
    }
    .container > div {
        flex-grow: default;
        width: 100%;
    }
}
</style>