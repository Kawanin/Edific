<template>
    <div class="card-container">
        
        <div class="image-container">
            <img :src="image" :alt="imageDescription">
        </div>
       

        <div class="text-container">
            <h2 class="title">{{ title }}</h2>
            <p class="subtitle">{{ subtitle }}</p>
        </div>

        <SaibaMaisButton class="button"/>
    </div>
</template>

<script setup>
import SaibaMaisButton from './SaibaMaisButton.vue'

defineProps({
    image: {
        image: String,
        required: true
    },
    title: {
        type: String,
        required: true
    },
    subtitle: {
        type: String,
        required: true
    },
})
</script>



<style scoped>
.card-container{
    max-width: 320px;
    text-align: center;
    padding: 40px 16px;
    position: relative;
    border-radius: 20px;
    box-shadow: 0px 7px 19px -8px rgba(0,0,0,0.15);
    display: flex;
    flex-direction: column;
    align-items: center;

    height: 440px;
}
.image-container{
    height: 60px;
    fill: #30AAB7;
    position: relative;
}
.image-container > img{
    filter: brightness(0) saturate(100%) invert(58%) sepia(37%) saturate(742%) hue-rotate(137deg) brightness(92%) contrast(90%);
    height: 100%
}
.title{
    margin-top: 12px;
    margin-bottom: 16px;
    color: #000;
    font-weight: 600;
    font-size: 17px;
}
.subtitle{
    color: #4f4f4f;
    font-weight: 400;
}
.button{
    position: absolute;
    bottom: 0;
    margin-bottom: 40px;
}
</style>