<template>
    <section class="bg-dark">
        <div class="container d-flex justify-content-between align-items-center py-4">
            <div>
                <button class="btn btn-dark border border-2 border-primary p-2">
                    <h5 class="text-white">SIGN-UP NOW!</h5>
                </button>
            </div>
            <div class="d-flex justify-content-center align-items-center gap-3">
                <div><a href=""><h5 class="text-primary fw-bold">FOLLOW US</h5></a></div>
                <div v-for="item in socialItems"><a href="#"><img :src="item"></a></div>
            </div>
        </div>
    </section>
    <!-- Footer Background Black -->
    <section class="bg-black py-3"></section>
</template>

<script>
export default{
    data() {
        return {
            socialItems: [
                "../../public/img/footer-facebook.png",
                "../../public/img/footer-periscope.png",
                "../../public/img/footer-pinterest.png",
                "../../public/img/footer-twitter.png",
                "../../public/img/footer-youtube.png",
            ],
        }
    },
}
</script>

<style scoped>
</style>
