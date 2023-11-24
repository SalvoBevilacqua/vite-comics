<script>
export default {

}
</script>

<template>
    <div class="container">
        footer dw
    </div>
</template>

<style scoped lang="scss">
@use "../style/partials/mixin" as *;
@use "../style/partials/variables" as *;

.container {
    height: 150px;
    color: white;
    @include flex();
}
</style>