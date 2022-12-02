<template>
    <footer class="bg-footer">
        <div class="container">
            <div class="text-white">
                <div>
                    <ul>
                        <li>
                            <h4>DC Comics</h4>
                            <div v-for="itemList in footerList">
                                <a href="#">{{itemList}}</a>
                            </div>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </footer>
</template>

<script>
export default{
    data() {
        return {
            footerList: ["Characters", "Comics", "Movies", "TV", "Games", "Videos", "News"],
        }
    },
}
</script>

<style scoped>
.bg-footer {
    background-image: url("../../public/img/footer-bg.jpg");
    background-size: cover;
    background-repeat: no-repeat;
}
</style>
