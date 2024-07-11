<template>
    <div @click="openButton">
        <span>Saiba Mais</span>
    </div>
</template>

<script setup>
const props = defineProps({
    message: {
        type: String,
    }
})

function openButton(){
    let string = props.message;
    let newString = string.replace(/\s/g, "%20");

    window.open('https://api.whatsapp.com/send?phone=5541987517945&text=' + newString, '_blank')
}
</script>


<style scoped>
div{
    font-size: 16px;
    font-weight: 500;
    text-shadow: 0px 0px 0px rgba(0, 0, 0, 0);
    fill: #fff;
    color: #fff;
    background-color: transparent;
    background-image: linear-gradient(180deg, #30AAB7 0%, #35bac9 100%);
    border-radius: 15px;
    width: fit-content;
    padding: 12px 24px;

    transition: .3s ease-out;
    display: inline-block;
    text-decoration: none; 
    cursor: pointer;
}
a:hover{
    transform: translate(0, -8px);
}
</style>