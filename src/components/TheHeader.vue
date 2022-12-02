<template>
    <header>
        <div class="nav-bg-black"></div>
        <div class="bg-light py-4">
            <div class="container">
                <nav class="d-flex justify-content-between align-items-center">
                    <div>
                        <img class="img-fluid" src="../../public/img/dc-logo.png" alt="DC-Comics-Logo">
                    </div>
                    <div class="nav-list">
                        <ul class="d-flex gap-4 fw-bold">
                            <li class="list-item" v-for="linkNavList in navList"><a href="#" class="text-dark">{{linkNavList}}</a></li>
                        </ul>
                    </div>
                </nav>
            </div>
        </div>
    </header>
</template>

<script>
export default {
    data() {
        return {
            navList: ["Characters", "Comics", "Movies", "TV", "Games", "Collectibles", "Videos", "Fans", "News", "Shop"],
        }
    },
}
</script>

<style scoped>
.nav-bg-black {
    background-color: black;
    height: 30px;
}

.list-item a:hover {
    border-bottom: 4px solid #0d6efd;
    color: #0d6efd !important;
    padding-bottom: 4.3rem;
}

/* .list-item a:nth-child(2){
    border-bottom: 4px solid #0d6efd;
    color: #0d6efd !important;
    padding-bottom: 4.3rem;
} */
</style>
