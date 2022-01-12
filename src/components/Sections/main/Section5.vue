<template>
    <div id="section-5">
        <div class="img-container">
            <img src="../../../assets/Img/h1-team-1a-700x700.jpg" alt="team">
        </div>
        <div class="img-container">
            <img src="../../../assets/Img/h1-team-2a.jpg" alt="team">
        </div>
        <div class="img-container">
            <img src="../../../assets/Img/h1-team-3a.jpg" alt="team">
        </div>
        <div class="img-container">
            <img src="../../../assets/Img/h1-team-4a.jpg" alt="team">
        </div>

    </div>
</template>

<script>
export default {
    name:"Section5"
}
</script>

<style lang="scss" scoped>
    #section-5 {
        display: flex;
        .img-container {
            width: 25%;
            margin: 0px 2px;
            img {
                width: 100%;
                // object-fit: cover;
            }
        }
    }
</style>