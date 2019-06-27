<template>
    <nav class="nav">

        <!-- upper half of nav housing the logo and searchbar -->
        <div class="nav-upper">
            <div class="Logo-circle"></div>
            <!-- <div class="nav-logo-wrapper">
                <a href="#" class="nav-logo-link">
                    <img src="~/assets/images/logo.png" />
                </a>
            </div> -->
            <img class="nav-search-img" src="~/assets/images/search.svg" /> 
        </div>

        <!-- lower half of nav for links  -->
        <div class="nav-lower">
            <div class="nav-links">
                <a href="">Home</a>
                <a href="">Guides</a>
                <a href="">News</a>
                <a href="">About</a>
            </div>
        </div>

    </nav>
</template>

<script>
export default {
    data() {
        return {

        }
    }

}
</script>

<style lang="scss" scoped>
@import "~/assets/scss/main.scss";
.Logo-circle {
    width: 40px;
    height: 40px;
    border-radius: 100%;
    background: linear-gradient(0.25turn, $m-pink, $m-orange);
    img {
        width: 45px;
        height: 45px;
        border-radius: 100%;
        transform:translateX(3px);
    }
}
.nav {
    display: flex;
    flex-direction: column;
    justify-content: center;
    background-color: white;
    padding: 0 20px 0 20px;

    .nav-upper {
        display: flex;
        align-items: center;
        justify-content: space-between;
        height: 56px;

        .nav-logo-wrapper {
            a {
                color: black;
            }
            .nav-logo-link {
                display: flex;
                align-items: center;
                img {
                    width: 45px;
                    height: 45px;
                    margin: 0 10px 0 0;
                }
            }
        }
         .nav-search-img {
            width: 15px;
            height: 15px;
        }
    }
    .nav-lower {
        .nav-links {
            display: flex;
            align-items: center;
            justify-content: space-between;
            text-transform: uppercase;
            height: 45px;
            a {
                font-size: 15px;
                color: rgba(0, 0, 0, 0.54);
                // margin: 0 0 0 24px;
            }
        }
    }
}

</style>
