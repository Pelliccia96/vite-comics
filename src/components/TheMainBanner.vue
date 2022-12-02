<template>
    <div class="bg-primary">
        <div class="container d-flex justify-content-between py-5">
            <div v-for="itemBanner in itemsList" class="d-flex align-items-center gap-2">
                <div class="img-container">
                    <img :src="itemBanner.img" class="img-fluid">
                </div>
                <div><a href="#" class="text-white">{{itemBanner.title}}</a></div>
            </div>
        </div>
    </div>
</template>

<script>
export default{
    data() {
        return {
            itemsList: [
                {
                    img: "../../public/img/buy-comics-digital-comics.png",
                    title: "Digital Comics",
                },
                {
                    img: "../../public/img/buy-comics-merchandise.png",
                    title: "DC Merchandise",
                },
                {
                    img: "../../public/img/buy-comics-subscriptions.png",
                    title: "Subscription",
                },
                {
                    img: "../../public/img/buy-comics-shop-locator.png",
                    title: "Comic Shop Locator",
                },
                {
                    img: "../../public/img/buy-dc-power-visa.svg",
                    title: "DC Power Visa",
                },
            ],
        }
    },
}
</script>

<style scoped>
img {
    display: block;
    width: 50px;
}
</style>
