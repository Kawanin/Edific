<template>
    <div class="container">
        <div class="enterprise-logo">
            <img :src="enterpriseLogo" alt="">
        </div>
        <div class="social-network">
            <div>
                <EmailIcon class="icon"/>
                <span>{{ email }}</span>
            </div>
            <div>
                <InstagramIcon class="icon"/>
                <span>{{ instagram }}</span>
            </div>
            <div>
                <WhatsAppIcon class="icon"/>
                <span>{{ whatsapp }}</span>
            </div>
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
</script>

<style scoped>
.container {
    width: 100vw;
    background-color: #0D0703;
    height: 250px;
    color: #FFFFFF;
    display: flex;


    position: absolute;
    top: 0;
    left: 0;
}
.container > div{
    flex-grow: 1;
    width: 50%;
    border: solid red 1px;
}
.enterprise-logo > img{
    width: 100%;
}

.icon{
    height: 25px;
    width: fit-content;
    filter: brightness(100);
    fill: #FFFFFF;
    margin-right: 8px;
}
.social-network{
    display: flex;
    flex-direction: column;
    justify-content: center;
    
}
.social-network > div{
    height: 50px;
    width: 100%;
    display: flex;
    align-items: center;
    background-color: red;
}
</style>