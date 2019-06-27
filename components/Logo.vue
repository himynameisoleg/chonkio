<template>
    <div class="Logo-container">
        <div class="Logo-circle"/>
    </div>
</template>

<style lang="scss" scoped>
@import "~/assets/scss/main.scss";

.Logo-container {
    display: flex;
    justify-content: center;

    .Logo-circle {
        width: 100px;
        height: 100px;
        border-radius: 100%;
        background: linear-gradient(0.25turn, $m-pink, $m-orange);
    }

}


</style>
