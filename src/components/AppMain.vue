<script>
import AppCard from "./AppCard.vue";

export default {
    data() {
        return {
            list: rows
        }
    },
    components: { AppCard }
}
</script>

<template>
    <div class="container">
        <span class="current">CURRENT SERIES</span>
        <main>
            <div class="row">
                <div class="col" v-for="item in list" :key="item.series">
                    <AppCard :name="item.series" :img="item.thumb" />
                </div>
            </div>
        </main>
    </div>
</template>

<style scoped lang="scss">
@use "../style/partials/mixin" as *;
@use "../style/partials/variables" as *;

.container {
    position: relative;

    .current {
        position: absolute;
        left: 0;
        top: 0;
        display: inline-block;
        padding: 1rem;
        background-color: $primary_color;
        color: white;
        transform: translateY(-50%);
    }

    main {
        width: 100%;
        padding: 3rem .75rem;
        color: white;

        .row {
            display: flex;
            justify-content: space-between;
            align-items: stretch;
            flex-wrap: wrap;

            .col {
                width: calc(100% / 6 - 0.75rem);
                margin-bottom: 1.5rem;
            }
        }
    }
}
</style>