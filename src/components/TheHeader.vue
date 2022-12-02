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
                            <li class="list-item" v-for="linkNavList in navList"><a href="#">{{linkNavList}}</a></li>
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

.list-item {
    list-style: none;
}
.list-item a:hover {
    border-bottom: 3px solid blue;
}
</style>
