<script>
export default {
    data() {
        return {
            listIcons: ["./src/assets/img/footer-facebook.png", "./src/assets/img/footer-twitter.png", "./src/assets/img/footer-youtube.png", "./src/assets/img/footer-pinterest.png", "./src/assets/img/footer-periscope.png"]
        }
    }
}
</script>

<template>
    <div class="container">
        <button type="button">SIGN-UP NOW!</button>

        <div class="icons">
            <button type="button">FOLLOW US</button>
            <a v-for="item in listIcons" href="">
                <img :src="item" alt="social">
            </a>
        </div>
    </div>
</template>

<style scoped lang="scss">
@use "../style/partials/mixin" as *;
@use "../style/partials/variables" as *;

.container {
    padding: 3rem 0;
    color: white;
    @include flex();

    button {
        display: inline-block;
        color: white;
        padding: 1rem;
        border: 2px solid $primary_color;
        background-color: $background_footer;
    }

    .icons {
        @include flex();
        gap: 1rem;

        button {
            color: $primary_color;
            display: inline-block;
            padding: 0;
            border: none;
        }
    }
}
</style>