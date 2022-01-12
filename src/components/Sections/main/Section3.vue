<template>
    <div id="section-3">
        <div class="left-column">
            <!-- <img src="../../../assets/Img/h1-img-4.jpg" alt=""> -->
            <img src="../../../assets/Img/h1-img-7n.png" alt="">
        </div>
        <div class="right-column">
            <div class="text-container">
                <h2>Specials*</h2>
                <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Libero officiis,</p>
                <div class="riga">
                    <div class="p-colonna">
                        <h3>$10</h3>
                    </div>
                    <div class="s-colonna">
                        <h3>Combo Piccolo</h3>
                        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Saepe omnis, officia fugiat soluta perferendis itaque at voluptates dolores nesciunt cum vero, consectetu</p>
                    </div>
                </div>
                <div class="riga">
                    <div class="p-colonna">
                        <h3>$10</h3>
                    </div>
                    <div class="s-colonna">
                        <h3>Combo Piccolo</h3>
                        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Saepe omnis, officia fugiat soluta perferendis itaque at voluptates dolores nesciunt cum vero, consectetu</p>
                    </div>
                </div>
                <div class="riga">
                    <div class="p-colonna">
                        <h3>$10</h3>
                    </div>
                    <div class="s-colonna">
                        <h3>Combo Piccolo</h3>
                        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Saepe omnis, officia fugiat soluta perferendis itaque at voluptates dolores nesciunt cum vero, consectetu</p>
                    </div>
                </div>
            </div>
            <div class="svg-pizza">
                    <img src="../../../assets/svg/svg-4.svg" alt="">
            </div>
        </div>
  </div>
</template>

<script>
export default {
    name: "Section3"

}
</script>

<style lang="scss" scoped>
    #section-3 {
        display: flex;
        

        .left-column, .right-column {
            width: 50%;
        }
        .left-column{
            position: relative;            
            background-image: url("../../../assets/Img/h1-img-4.jpg");
            background-repeat:no-repeat;

            img {
                // width: 100%;
                position: absolute;
                top: 50%;
                left: 50%;
                transform: translate(-50%,-50%);
            }
          
        }
        .right-column {
            // padding: 25px;
            // background-color: blue;
            position: relative;
            display: flex;
            .text-container {
                padding: 150px;
                border-color: red;
                width: 80%;
                h3, h2 {
                    text-transform: uppercase;
                }
                p{
                    color: grey;
                    font-size: 12px;
                    margin: 10px 0px;
                }
                .riga {
                    display: flex;
                    margin: 25px 0px;
                    .p-colonna {
                        h3 {
                            color: #C83B1A;
                        }
                    }
                    .s-colonna {
                        margin-left: 15px;
                    }
                }
            }

            .svg-pizza {
                position: absolute;
                bottom:250px;
                right: 10px;
                // background-color: blue;
            }
        }
    }
</style>