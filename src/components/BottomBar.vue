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
    width: 100%;
    height: 250px;
    background-color: #0D0703;
    color: #FFFFFF;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    position: relative;
}
.container {
    width: 100%;
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
    max-width: 300px;
    height: fit-content;
}

.icon {
    height: 25px;
    width: 25px;
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
.social-network > div:not(:first-of-type) {
    cursor: pointer;
}
.copyright-container{
   position: absolute;
   bottom: 0;
   padding: 20px;
   font-size: 13px;
}
@media (max-width: 760px) {
    .container{
        flex-direction: column;
        height: 350px;
        margin-bottom: 0px;
        width: 400px;
        position: relative;
        justify-content: center;
        align-items: center;
        margin-bottom: 40px;
        width: 100%;
    }
    .wrapper{
        height: 390px;
        position: relative;
    }
    .social-network {
        border-left: none;
        padding-left: 0;
        width: 10px;
        text-align: center;
        align-items: center;
    }
    .social-network > div{
        width: max-content;
    }
    .enterprise-logo{
        display: flex;
        justify-content: center;
        align-items: center;
        padding-right: 0;
    }
    .enterprise-logo > img {
        max-width: 300px;
    }
    .container > div {
        flex-grow: 0;
        width: 100%;
    }
    .social-network > span{
        border-top: 1px solid white;
        padding-top: 22px;
        margin-top: 18px;
        text-align: center;
        width: 280px;
    }
    .copyright-container{
        padding: 14px;
        text-align: center;
    }
}
</style>