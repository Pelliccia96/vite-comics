<template>
    <main class="bg-dark">
        <!-- Jumbotron -->
        <div class="main-bg"/>
        <div class="container">
            <div class="text-white d-flex margin-">
                <h3 class="border border-primary bg-primary rounded fw-bold p-3">CURRENT SERIES</h3>
            </div>
            <!-- Cards -->
            <div class="row row-cols-1 row-cols-md-3 row-cols-lg-6 g-4 my-3">
                <div class="col" v-for="(singleCard,i) in comicsList" :key="(singleCard.series + i)">
                    <CardComponent :card="singleCard"></CardComponent>
                </div>
            </div>
            <div class="text-center my-2">
                <button class="btn btn-primary fw-bold p-2 px-5 mb-4">LOAD MORE</button>
            </div>
        </div>
    </main>
</template>

<script>
import CardComponent from './CardComponent.vue';
import dcComics from '../dc-comics.js';

export default{
    components: { CardComponent },
    data() {
        return {
            comicsList: dcComics,
        }
    },
}
</script>

<style scoped>
.main-bg {
    background-image: url(../../public/img/jumbotron.jpg);
    background-size: cover;
    background-position: top;
    height: 400px;
}

.margin- {
    margin-top: -30px;
}
</style>
