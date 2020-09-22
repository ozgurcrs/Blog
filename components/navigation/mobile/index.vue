<template>
<div class="d-flex justify-content-end">
    <button @click="buttonClick = !buttonClick" class="btn button">
        <i v-if="!buttonClick" class="fas fa-bars"></i>
        <i v-else class="fas fa-times"></i>
    </button>
    <div v-if="buttonClick" class="navigation animate__animated animate__fadeInLeftBig">
        <ul @click="buttonClick = !buttonClick">
            <nuxt-link to="/" tag="li" exact active-class="active"><i class="fas fa-home fa-lg"><span> Home</span></i></nuxt-link>
            <nuxt-link to="/aboutMe" active-class="active" tag="li"><i class="fas fa-user fa-lg"><span> About</span></i></nuxt-link>
            <li>
                <a href="#"><i class="fas fa-id-badge fa-lg"> <span> Portfolio</span></i></a>
            </li>
            <li>
                <a href="#"><i class="fas fa-envelope-open fa-lg"><span> Contact</span></i></a>
            </li>
            <li>
                <a href="#"><i class="fas fa-comment-dots fa-lg"><span> my Blog</span></i></a>
            </li>
        </ul>
    </div>
</div>
</template>

<script>
export default {
    data() {
        return {
            buttonClick: false
        };
    }
};
</script>

<style scoped>
.button {
    padding: 10px;
    color: #fff;
    z-index: 2;
}

.button i {
    font-size: 24px;
    transition: 1s;
}

.btn:focus {
    box-shadow: none;
}

.navigation {
    position: absolute;
    left: 0;
    top: 0;
    width: 100%;
    height: 100vh;
    z-index: 1;
    background: rgb(51, 51, 51, 0.90);
}

.navigation ul {
    width: 100%;
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    padding-right: 20px;
}

.navigation ul li {
    width: 100%;
    padding: 20px;
    list-style: none;
    height: auto;
    margin: 5px 0;
    transition: 300ms;
}

.navigation span {
    font-family: "Raleway", sans-serif;
    letter-spacing: 3px;
    padding-left: 5px;
}

.navigation a {
    color: #fff;
}

.active {
    border-bottom: 3px solid #f9b000;
    border-bottom-left-radius: 3px;
    border-bottom-right-radius: 3px;
}
</style>
