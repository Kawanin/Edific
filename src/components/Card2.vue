<template>
    <div class="container">
        <img :src="image" alt="">
        <div>
            <h3>{{ title }}</h3>
            <p>{{ description }}</p>
        </div>       
    </div>
</template>

<script setup>
defineProps({
    image: {
        image: String,
        required: true
    },
    title: {
        description: String,
        required: true
    },
    description: {
        description: String,
        required: true
    },
})
</script>


<style scoped>
.container{
    display: flex;
    flex-direction: row;
    height: 110px;
    max-width: 450px;
    padding: 18px 26px;
    align-items: center;
    color: #282828;
    background-color: #fff;
    border-radius: 16px;
    box-shadow: 3px 3px 26px -4px rgba(0,0,0,0.15);
    text-align: start;
}
.container > div > h3{
    font-weight: 700;
    font-size: 16px;
}
img{
    max-height: 100%;
    margin-right: 20px;
    filter: brightness(0) saturate(100%) invert(58%) sepia(37%) saturate(742%) hue-rotate(137deg) brightness(92%) contrast(90%);
}
@media (max-width: 470px) {
    .container{
        flex-direction: column;
        height: fit-content;
        align-items: center;
        text-align: center;
    }
    img{
        margin-right: 0px;
        width: 70px;
        margin-bottom: 20px;
    }
}
</style>
