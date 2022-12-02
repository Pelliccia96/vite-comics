<template>
    <footer class="bg-footer">
        <div class="container py-5 overflow-hidden">
            <div class="text-white d-flex gap-4">
                <div>
                    <ul>
                        <li class="list-item">
                            <h4>DC Comics</h4>
                            <div v-for="item in dcComicsList">
                                <a href="#">{{item}}</a>
                            </div>
                        </li>
                    </ul>
                    <ul>
                        <li class="list-item">
                            <h4>Shop</h4>
                            <div v-for="item in shopList">
                                <a href="#">{{item}}</a>
                            </div>
                        </li>
                    </ul>
                </div>
                <div class="d-flex gap-3">
                    <ul>
                        <li class="list-item">
                            <h4>DC</h4>
                            <div v-for="item in dcList">
                                <a href="#">{{item}}</a>
                            </div>
                        </li>
                    </ul>
                    <ul>
                        <li class="list-item">
                            <h4>Sites</h4>
                            <div v-for="item in sitesList">
                                <a href="#">{{item}}</a>
                            </div>
                        </li>
                    </ul>
                </div>
                <!-- Footer DC Logo bg -->
                <div class="footer-logo-bg">
                    <img src="../../public/img/dc-logo-bg.png" alt="DC Logo in background">
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default{
    data() {
        return {
            dcComicsList: ["Characters", "Comics", "Movies", "TV", "Games", "Videos", "News"],
            shopList: ["Shop Dc", "Shop Dc Collectibles"],
            dcList: ["Term Of Use", "Privacy policy (New)", "Ad Choise", "Adversting", "Jobs", "Subscriptions", "Talent Workshops", "CPSC Certificateds", "Rating", "Shop Help", "Contact Us"],
            sitesList: ["DC", "MAD Magazine", "DC Kids", "DC Universe", "DC Power Visa",],
        }
    },
}
</script>

<style scoped>
a {
    font-size: small;
    color: grey;
}
.bg-footer {
    background-image: url("../../public/img/footer-bg.jpg");
    background-size: cover;
    background-repeat: no-repeat;
}

.footer-logo-bg {
    margin-top: -100px;
    margin-bottom: -200px;
    padding-left: 200px;
}
</style>
