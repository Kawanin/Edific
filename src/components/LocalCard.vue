<template>
    <div class="local-card-container">
        <div class="text-container">
            <p class="title">{{ title }}</p>
            <p>{{ subtitle }}</p>
            <p>Telefone: {{ telephone }}</p>
        </div>
        <img :src="image" alt="Google Maps" @click="openGoogleMaps">
    </div>
</template>

<script setup>
defineProps({
    title: {
        type: String,
        required: true
    },
    subtitle: {
        type: String,
        required: true
    },
    telephone: {
        type: String,
        required: true
    },
    image: {
        type: String,
        required: true
    },
})

function openGoogleMaps() {
    window.open('http://google.com','_blank')
}
</script>

<style scoped>
.local-card-container{
    max-width: 540px;
    height: fit-content;
    padding: 20px;
    border-radius: 24px;
    text-align: center;
    box-shadow: 0px 0px 10px 0px rgba(0, 0, 0, .17);
}
.text-container{
    padding-bottom: 8px;
}
p{
    padding-bottom: 10px;
}
.title{
    padding-bottom: 8px;
    font-weight: bold;
    font-size: 16px;
}
img{
    width: 100%;
    cursor: pointer;
}

</style>

