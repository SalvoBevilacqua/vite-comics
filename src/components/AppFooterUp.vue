<script>
export default {

}
</script>

<template>
    <div class="container">
        footer up
    </div>
</template>

<style scoped lang="scss">
@use "../style/partials/mixin" as *;
@use "../style/partials/variables" as *;

.container {
    height: 450px;
    color: white;
    @include flex();
}
</style>