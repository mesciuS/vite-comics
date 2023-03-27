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
        <img :src="img" alt="">
        <div class="card-title">{{ serie }}</div>
    </div>
</template>

<style lang="scss" scoped>
.card {
    display: flex;
    flex-direction: column-reverse;
    width: 200px;
    height: 250px;
    border: 1px solid red;

    .card-title {
        padding-top: 20px;
    }

    img {
        width: 100%;
    }
}
</style>