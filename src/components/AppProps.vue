<script>
export default {
    data() {
        return {
            
        }
    },

    props: {
        img: String,
        prezzo: String,
        serie: String,
        tipo: String,
    },
}
</script>

<template>
    <div class="card">
        <div class="img-wrapper">
            <img :src="img" alt="">
        </div>
        <div class="card-title">{{ serie }}</div>
    </div>
</template>

<style lang="scss" scoped>
.card {
    display: flex;
    flex-direction: column;

    .img-wrapper {
        width: 200px;
        height: 250px;
    }

    .card-title {
        width: 200px;
        padding-top: 20px;
        word-wrap: break-word;
    }

    img {
        width: 100%;
        height: 100%;
    }
}
</style>