<script>
export default {
    data() {
        return {
            listInfo: [
                { name: "DIGITAL COMICS", url: "./src/assets/img/buy-comics-digital-comics.png", },
                { name: "DC MERCHANDISE", url: "./src/assets/img/buy-comics-merchandise.png", },
                { name: "SUBSCRIPTION", url: "./src/assets/img/buy-comics-subscriptions.png", },
                { name: "COMIC SHOP LOCATOR", url: "./src/assets/img/buy-comics-shop-locator.png", },
                { name: "DC POWER VISA", url: "./src/assets/img/buy-dc-power-visa.svg", },
            ]
        }
    }
}
</script>

<template>
    <div class="container">
        <ul>
            <li v-for="image in listInfo" :key="image.name">
                <img :src="image.url" :alt="image.name">
                <p>{{ image.name }}</p>
            </li>
        </ul>
    </div>
</template>

<style scoped lang="scss">
@use "../style/partials/mixin" as *;
@use "../style/partials/variables" as *;

.container {
    padding: 3rem 1.5rem;
    color: white;

    ul {
        @include flex();

        li {
            @include flex();

            img {
                height: 65px;
            }
        }
    }
}
</style>