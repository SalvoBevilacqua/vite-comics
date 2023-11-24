<script>
export default {
    data() {
        return {
            listItems: [
                { name: "CHARACTER", active: false, },
                { name: "COMICS", active: true, },
                { name: "MOVIES", active: false, },
                { name: "TV", active: false, },
                { name: "GAMES", active: false, },
                { name: "COLLECTIBLES", active: false, },
                { name: "VIDEOS", active: false, },
                { name: "FANS", active: false, },
                { name: "NEWS", active: false, },
                { name: "SHOP", active: false, },
            ]
        }
    }
}
</script>

<template>
    <div class="container">
        <header>
            <img src="../assets/img/dc-logo.png" alt="logo dc">

            <ul>
                <li v-for="item in listItems" :key="item.name"><span><a href="">{{ item.name }}</a></span></li>
            </ul>
        </header>
    </div>
</template>

<style scoped lang="scss">
@use "../style/partials/mixin" as *;
@use "../style/partials/variables" as *;

header {
    width: 100%;
    height: 150px;
    @include flex();

    img {
        height: 70%;
        aspect-ratio: 1;
    }

    ul {
        @include flex();
        list-style: none;
        gap: 1.5rem;

        li {
            span {
                display: inline-block;
                height: 150px;
                line-height: 150px;

                &:hover {
                    border-bottom: 5px solid $primary_color;
                    color: $primary_color;
                }

                a {
                    text-decoration: none;
                    color: inherit;
                }
            }
        }
    }
}
</style>