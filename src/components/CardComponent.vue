<template>
    <div class="card border-0">
        <img :src="card.thumb" class="card-img-top">
        <div class="card-body bg-dark">
            <h5 class="card-title text-white">{{card.series}}</h5>
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
</style>
