<template>
    <div class="card border-0">
        <img :src="card.thumb" class="card-img-top">
        <div class="card-body bg-dark">
            <h6 class="card-title text-white">{{card.series}}</h6>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        card: {
            type: Object,
            required: true,
        }
    },
}
</script>

<style scoped>
.card-img-top:hover {
    opacity: 50%;
}

img {
    aspect-ratio: 1 / 1;
    object-fit: cover;
    object-position: top;
}
</style>
