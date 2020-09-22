<template>
<div class="appCard">
    <appCard v-for="item in 3" :key="item" />
</div>
</template>

<script>
import appCard from './card';
export default {
    components: {
        appCard
    }
}
</script>

<style scoped>
.appCard {
    width: 100%;
    height: 100vh;
    display: flex;
    flex-direction: column;
    align-items: center;
    margin-top: 20px;
}
</style>
