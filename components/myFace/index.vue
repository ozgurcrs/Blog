<template>
<div class="leftContainer">
    <div class="leftContainerBg"></div>
    <div class="containerImage shadow">
        <img class="shadow" src="@/static/myImage/myPhoto.jpg" alt="" />
    </div>
</div>
</template>

<style scoped>
.leftContainer {
    width: 80%;
    height: 100vh;
    display: flex;
    justify-content: center;
    align-items: center;
    overflow: hidden;
    padding: 40px;

}

.leftContainerBg {
    width: 25%;
    height: 120%;
    position: fixed;
    overflow: hidden;
    z-index: -1;
    left: -8%;
    top: -3%;
    background: #F9B000;
    transform: rotate(-8deg);
}

.containerImage {
    border-radius: 10px;
}

.containerImage img {
    border-radius: 10px;
    width: 100%;
    height: auto;
    filter: grayscale(100%);
    transition: 1s;
}

.containerImage img:hover {
    filter: grayscale(0%);
}
</style>
