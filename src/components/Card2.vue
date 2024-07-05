<template>
    <div>
        <img :src="image" :alt="imageDescription">
        <p>{{ description }}</p>
    </div>
</template>

<script setup>
defineProps({
    image: {
        image: String,
        required: true
    },
    description: {
        description: String,
        required: true
    },
    subtimageDescriptionitle: {
        description: String,
        required: false
    }
})
</script>


<style scoped>
div{
    display: flex;
    flex-direction: row;
    height: 110px;
    max-width: 480px;
    padding: 10px;
    color: white;
    align-items: center;
    color: #282828;
}
div > p{
    height: fit-content;
}
img{
    max-height: 100%;
    margin-right: 20px;
    filter: brightness(0) saturate(100%) invert(58%) sepia(37%) saturate(742%) hue-rotate(137deg) brightness(92%) contrast(90%);
    filter: brightness(0) saturate(100%) invert(64%) sepia(83%) saturate(2918%) hue-rotate(326deg) brightness(89%) contrast(95%);
}
@media (max-width: 420px) {
    div{
        flex-direction: column;
        height: fit-content;
        align-items: center;
        text-align: center;
    }
    img{
        margin-right: 0px;
        width: 45vw;
        margin-bottom: 20px;
    }
}
</style>
