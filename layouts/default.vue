<template>
    <div>
        <Navbar/>
        <nuxt/>
    </div>
</template>

<script>
import Navbar from "@/components/Navbar"

export default {
    components: {
		Navbar
	}
};
</script>


<style lang="scss">
@import "~/assets/scss/main.scss";
html {
    font-family: 'Open Sans', Arial, sans-serif;
    font-size: 16px;
    word-spacing: 1px;
    -ms-text-size-adjust: 100%;
    -webkit-text-size-adjust: 100%;
    -moz-osx-font-smoothing: grayscale;
    -webkit-font-smoothing: antialiased;
    box-sizing: border-box;

	background: linear-gradient(0.1turn, $m-purple, $m-yellow);
	background-repeat: no-repeat;
	
}
body {
    font-family: 'Open Sans', Arial, sans-serif;
}
*,
*:before,
*:after {
    box-sizing: border-box;
    margin: 0;
}


</style>
