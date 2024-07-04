<template>
    <div class="card-container">
        
        <div class="svg-container">
            
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
    padding: 66px 16px;
    position: relative;
    border-radius: 20px;
    box-shadow: 0px 7px 19px -8px rgba(0,0,0,0.15);
    display: flex;
    flex-direction: column;
}
.svg{
    height: 50px;
    width: 50px;
    fill: #30AAB7;
}
.text-container{
    margin-bottom: 30px
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
</style>