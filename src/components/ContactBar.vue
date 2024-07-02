<template>
    <div class="contact-bar-container">
        <div class="email-container">
            <div>
                <EmailIcon class="icon"/>
                <span>{{ email }}</span>
            </div>
        </div>
        <div class="telephone-container">
            <div @click="openWhatsapp">
                <TelephoneIcon class="icon"/>
                <span>{{ telephone }}</span>
            </div>
        </div>
        <div class="instagram-container">
            <div @click="openInstagram">
                <InstagramIcon class="icon"/>
                <span>{{ instagram }}</span>
            </div>
        </div>
    </div>
</template>

<script setup>
import EmailIcon from './icons/EmailIcon.vue'
import TelephoneIcon from './icons/TelephoneIcon.vue'
import InstagramIcon from './icons/InstagramIcon.vue'

defineProps({
    email: {
        type: String,
        required: true
    },
    telephone: {
        type: String,
        required: true
    },
    instagram: {
        type: String,
        required: true
    },

    
})

function openWhatsapp() {
    window.open('http://google.com','_blank')
}
function openInstagram() {
    window.open('http://google.com','_blank')
}
</script>

<style scoped>
.contact-bar-container{
    width: 100vw;
    height: 43px;
    display: flex;
    flex-wrap: wrap;
    box-shadow: 0px 0px 29px -16px rgba(0,0,0,0.75);
}
.contact-bar-container > div{
    flex-grow: 1;
    width: 33%;
    display: flex;
    justify-content: center;
    align-items: center;
}
.contact-bar-container > div > div{
    display: flex;
    justify-content: center;
    align-items: center;
    width: fit-content;
    height: 100%;
    padding: 0px 28px;
    cursor: pointer;
}
.icon{
    width: 24px;
    height: 24px;
    margin-right: 10px;
}

@media (max-width: 890px) {
  .contact-bar-container > div{
    width: initial;
  }
}

@media (max-width: 760px) {
    .contact-bar-container{
        flex-direction: column;
        flex-wrap: nowrap;
        height: 130px;
    }
}
</style>

