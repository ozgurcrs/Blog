<template>
<div class="navigation">
    <ul>

        <nuxt-link to="/" tag="li" exact active-class="active"><i class="fas fa-home fa-lg"></i></nuxt-link>
        <nuxt-link to="/aboutMe" active-class="active" tag="li"><i class="fas fa-user fa-lg"></i></nuxt-link>

        <li>
            <a href="#"><i class="fas fa-id-badge fa-lg"></i></a>
        </li>
        <li>
            <a href="#"><i class="fas fa-envelope-open fa-lg"></i></a>
        </li>
        <li>
            <a href="#"><i class="fas fa-comment-dots fa-lg"></i></a>
        </li>
    </ul>
</div>
</template>

<style scoped>
.navigation {
    height: 100vh;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
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

.navigation a {
    color: #fff;
}

.active {
    border-bottom: 3px solid #f9b000;
    border-bottom-left-radius: 3px;
    border-bottom-right-radius: 3px;
}

.navigation ul li:hover {
    border-bottom: 3px solid #333;
    border-bottom-left-radius: 3px;
    border-bottom-right-radius: 3px;
}
</style>
