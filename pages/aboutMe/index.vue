<template>
<div class="aboutContainer animate__animated animate__fadeInDown">
    <h2>About Me</h2>

    <div class="listContainer">
        <ul>
            <li>
                <i class="far fa-dot-circle"></i> First Name: <span>Özgür</span>
            </li>
            <li><i class="far fa-dot-circle"></i> Last Name: <span>Çiriş</span></li>
            <li><i class="far fa-dot-circle"></i> Age: <span>25 Years</span></li>

            <li><i class="far fa-dot-circle"></i> Country : <span>Turkey</span></li>
            <li><i class="far fa-dot-circle"></i> City : <span>Istanbul</span></li>
        </ul>
        <ul>
            <li>
                <i class="far fa-dot-circle"></i> School:
                <span>Istanbul Commerce University</span>
            </li>
            <li>
                <i class="far fa-dot-circle"></i> Education:
                <span>Computer Engineering</span>
            </li>
            <li>
                <i class="far fa-dot-circle"></i> Experience:
                <span>Frontend Developer</span>
            </li>
            <li>
                <i class="far fa-dot-circle"></i> Email :
                <span>ozgurciris@gmail.com</span>
            </li>
            <li>
                <i class="far fa-dot-circle"></i> Phone : <span>539-583-63-65</span>
            </li>
        </ul>
    </div>

    <ul>
        <li>
            <p> I'm a Turkey based web designer & front‑end developer focused on crafting
                clean & user‑friendly experiences, I am passionate about building
                excellent software that improves the lives of those around me. &#128151</p>
        </li>
    </ul>

    <div class="button">
        <button class="button btn btn-warning">Download CV</button>
    </div>
</div>
</template>

<script>
export default {};
</script>

<style scoped>
.aboutContainer {
    width: 100%;
    height: 90vh;
    display: flex;
    align-items: center;
    justify-content: space-around;
    font-family: "Raleway", sans-serif;
    flex-direction: column;

}

.aboutContainer h2 {
    width: 70%;
    text-align: center;
    padding: 10px;

}

.listContainer {
    width: 100%;
    height: auto;
    display: flex;
    align-items: center;
    justify-content: space-around;
}

.aboutContainer li {
    list-style: none;
    color: rgb(135, 135, 135);
    font-size: 14px;
    letter-spacing: 1px;
    line-height: 40px;
    text-align: left;

}

.aboutContainer span {
    color: rgb(228, 228, 228);
}
</style>
