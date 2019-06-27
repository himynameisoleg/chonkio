<template>
    <section class="section">
        <div class="container">
            <div>
                <!-- <logo/> -->
                <h1 class="title">chonk.io</h1>
                <h2 class="subtitle">{{ `dedicated to eveything \nclick, clack and chonk` }}</h2>
            </div>

            <div class="">

            </div>
        </div>
    </section>
</template>

<script>
import Logo from "~/components/Logo.vue";

export default {
    components: {
        Logo
    }
};
</script>

<style lang="scss" scoped>
@import "~/assets/scss/main.scss";
.section {
    box-shadow: 0 4px 12px 0 rgba(0, 0, 0, 0.05) inset;
}
.container {
    margin: 0 auto;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 24px;
    
    h1 {
        color: white;
        font-size: 32px;
    }
    h2 {
        color: white;
        white-space:pre-wrap;
    }
}
</style>
