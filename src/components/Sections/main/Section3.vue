<template>
    <div id="section-3" class="container-fluid">
        <div class="row">
            <div class="left-column col-lg-6 col-md-12">
                <img class='back' src="../../../assets/Img/h1-img-4.jpg" alt="">
                <img class='front' src="../../../assets/Img/h1-img-7n.png" alt="">
            </div>
            <div class="right-column col-lg-6 col-md-12">
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
        .left-column{
            position: relative;       
            padding: 0;     
            .back {
                width: 100%;
            }
            .front {
                position: absolute;
                top: 50%;
                left: 50%;
                transform: translate(-50%,-50%);
            }
        }
        .right-column {
            padding: 0;
            display: flex;
            .text-container {
                padding: 100px;
                border-color: red;
                // width: 80%;
                h3, h2 {
                    text-transform: uppercase;
                    font-weight: bold;
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
        }
    }
</style>