<script>
export default {
    data() {
        return {
            buyObjects: [
            {
                title: "Digital Comics",
                img: "buy-comics-digital-comics.png"
            },
            {
                title: "DC Merchandise",
                img: "buy-comics-merchandise.png"
            },
            {
                title: "Subscription",
                img: "buy-comics-subscriptions.png"
            },
            {
                title: "Comic Shop Locator",
                img: "buy-comics-shop-locator.png"
            },
            {
                title: "DC Power Visa",
                img: "buy-dc-power-visa.svg"
            },
            ]

        }
    }
}
</script>

<template>
    <div id="shop-container">
        <a href="#" class="shop-element">
            <img src="/img/buy-comics-digital-comics.png" alt="" class="icon">
            <span class="title">titolo</span>
        </a>
        <a href="#" class="shop-element">
            <img src="/img/buy-comics-digital-comics.png" alt="" class="icon">
            <span class="title">titolo</span>
        </a>
        <a href="#" class="shop-element">
            <img src="/img/buy-comics-digital-comics.png" alt="" class="icon">
            <span class="title">titolo</span>
        </a>
        <a href="#" class="shop-element">
            <img src="/img/buy-comics-digital-comics.png" alt="" class="icon">
            <span class="title">titolo</span>
        </a>
        <a href="#" class="shop-element">
            <img src="/img/buy-comics-digital-comics.png" alt="" class="icon">
            <span class="title">titolo</span>
        </a>
        
    </div>
</template>

<style lang="scss" scoped>
#shop-container {
    display: none;
}
</style>