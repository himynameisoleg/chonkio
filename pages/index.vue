<template>
    <div class="container">
        <div>
            <logo/>
            <h1 class="title">Clack</h1>
            <h2 class="subtitle">My Clack Proj</h2>
        </div>
    </div>
</template>

<script>
import Logo from "~/components/Logo.vue";

export default {
    components: {
        Logo
    }
};
</script>

<style lang="scss">
.container {
    margin: 0 auto;
    min-height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 0 24px 0 24px;
    box-shadow: 0 4px 12px 0 rgba(0, 0, 0, 0.05) inset;
    background-color: white;
}

.title {
    font-family: "Quicksand", "Source Sans Pro", -apple-system,
        BlinkMacSystemFont, "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
    display: block;
    font-weight: 300;
    font-size: 100px;
    color: #35495e;
    letter-spacing: 1px;
}

.subtitle {
    font-weight: 300;
    font-size: 42px;
    color: #526488;
    word-spacing: 5px;
    padding-bottom: 15px;
}

.links {
    padding-top: 15px;
}
</style>
