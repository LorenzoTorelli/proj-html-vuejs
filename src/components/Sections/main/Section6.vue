<template>
    <div id="sezione-6">
        <div class="container-top">
            <div class="container-logo">
                <img src="../../../assets/Img/h1-clients-img-1.png" alt="">
            </div>
            <div class="container-logo">
                <img src="../../../assets/Img/h1-clients-img-2.png" alt="">
            </div>
            <div class="container-logo">
                <img src="../../../assets/Img/h1-clients-img-3.png" alt="">
            </div>
            <div class="container-logo">
                <img src="../../../assets/Img/h1-clients-img-4.png" alt="">
            </div>
            <div class="container-logo">
                <img src="../../../assets/Img/h1-clients-img-5.png" alt="">
            </div>
        </div>
        <div class="container-bottom">
            <div>
                <h5>choose your flavor</h5>
                <h4>The best pizza menu in town</h4>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Deserunt est molestiae eaque cum provident, consectetur repellat dolore.</p>
            </div>
        </div>
         <div class="svg-pizza">
            <img src="../../../assets/svg/svg-4.svg" alt="">
        </div>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
    #sezione-6 {
        margin: 100px 0px;
        position: relative;
        .container-top {
            display: flex;
            width: 70%;
            margin: auto;
        }

        .container-bottom {
            margin: 150px;
            div {
                width: 50%;
                margin: auto;
                text-align: center;

                h5 {
                    color: red;
                    text-transform: uppercase;
                }
                h4 {
                    font-size: 30px;
                    text-transform: uppercase;
                    margin-bottom:15px ;
                }
                p {
                    color: grey;
                }
            }

        
        }
        .svg-pizza {
            position: absolute;
            right: 1%;
            bottom: 10%;
        }
    }
</style>