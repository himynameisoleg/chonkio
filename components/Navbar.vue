<template>
    <nav class="navbar has-background-white">
        <div class="navbar-brand">
            <a class="navbar-item" href="/">
                <div class="Logo-circle"></div>
            </a>
            <div
                class="navbar-burger"
                @click="showNav = !showNav"
                :class="{ 'is-active': showNav }"
            >
                <span></span>
                <span></span>
                <span></span>
            </div>
        </div>

        <div class="navbar-menu" :class="{ 'is-active': showNav }">
            <div class="navbar-end">
                <a class="navbar-item" href="/about">About</a>
                <a class="navbar-item" href="/path">Path</a>
                <a class="navbar-item" href="/blog">Blog</a>
            </div>
        </div>
    </nav>
</template>

<script>
export default {
    data() {
        return {
            showNav: false
        };
    }
};
</script>

<style lang="scss" scoped>
@import "~/assets/scss/main.scss";
.Logo-circle {
    width: 28px;
    height: 28px;
    // margin: 6px;
    border-radius: 100%;
    background: linear-gradient(0.25turn, $m-pink, $m-orange);
}
// .nav {
//     display: flex;
//     flex-direction: column;
//     justify-content: center;
//     background-color: white;
//     padding: 0 20px 0 20px;

//     .nav-upper {
//         display: flex;
//         align-items: center;
//         justify-content: space-between;
//         height: 56px;

//         .nav-logo-wrapper {
//             a {
//                 color: black;
//             }
//             .nav-logo-link {
//                 display: flex;
//                 align-items: center;
//                 img {
//                     width: 45px;
//                     height: 45px;
//                     margin: 0 10px 0 0;
//                 }
//             }
//         }
//          .nav-search-img {
//             width: 15px;
//             height: 15px;
//         }
//     }
//     .nav-lower {
//         .nav-links {
//             display: flex;
//             align-items: center;
//             justify-content: space-between;
//             text-transform: uppercase;
//             height: 45px;
//             a {
//                 font-size: 15px;
//                 color: rgba(0, 0, 0, 0.54);
//                 // margin: 0 0 0 24px;
//             }
//         }
//     }
// }
</style>
