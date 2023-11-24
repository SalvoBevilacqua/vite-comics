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
        <img :src="img" :alt="name">
        <p class="name">{{ name }}</p>
    </div>
</template>

<style scoped lang="scss">
@use "../style/partials/mixin" as *;
@use "../style/partials/variables" as *;

.card {
    height: 100%;

    img {
        width: 100%;
    }
}
</style>