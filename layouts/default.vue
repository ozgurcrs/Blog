<template>
<div class="myContainer" :class="!isMobile ? myContainer : ''">
    <myFace v-if="isMobile" />
    <navigationMobile v-else />
    <faceMobile v-if="!isMobile" />
    <nuxt />
    <appNavigation v-if="isMobile" />
</div>
</template>

<script>
import myFace from "@/components/myFace";
import faceMobile from "@/components/myFace/mobile";
import appNavigation from "@/components/navigation";
import navigationMobile from "@/components/navigation/mobile";
export default {
    components: {
        myFace,
        faceMobile,
        appNavigation,
        navigationMobile
    },

    data() {
        return {
            myContainer: {
                "d-flex": "d-flex",
                "flex-column": "flex-column"
            },
            isMobile: false
        };
    },

    mounted() {
        if (/Android|webOS|iPhone|iPad|iPod|BlackBerry|IEMobile|Opera Mini/i.test(navigator.userAgent))
            this.isMobile = false;
        else
            this.isMobile = true;
    },

};
</script>

<style>
/*

font-family: 'Playfair Display', serif;
font-family: 'Raleway', sans-serif;
font-family: 'Roboto', sans-serif;

*/

body {
    background: rgb(27, 27, 27);
    padding: 0;
    margin: 0;
    color: #fff;
}

.myContainer {
    display: flex;
}
</style>
