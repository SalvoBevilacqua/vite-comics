<script>
export default {

}
</script>

<template>
    <div class="container">
        <main>
            <span>Content goes here</span>
        </main>
    </div>
</template>

<style scoped lang="scss">
@use "../style/partials/mixin" as *;
@use "../style/partials/variables" as *;

main {
    width: 100%;
    height: 150px;
    color: white;
    @include flex();
}
</style>