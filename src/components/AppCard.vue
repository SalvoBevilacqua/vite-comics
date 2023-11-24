<script>
export default {
    props: {
        name: String,
        img: String,
    }
}
</script>

<template>
    <div class="card">
        <div class="image">
            <img :src="img" :alt="name">
        </div>
        <p class="name">{{ name }}</p>
    </div>
</template>

<style scoped lang="scss">
@use "../style/partials/mixin" as *;
@use "../style/partials/variables" as *;

.card {
    .image {
        width: 100%;
        aspect-ratio: 1;

        img {
            width: 100%;
            height: 100%;
            object-fit: cover;
            object-position: 50% 25%;
        }
    }
}
</style>