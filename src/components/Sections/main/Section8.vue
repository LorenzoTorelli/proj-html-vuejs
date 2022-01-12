<template>
    <div id="sezione-8" class="container-fluid">
        <div class="row">
            <div class="left-column col-lg-6 col-md-12 ">
                <div class="title">
                    <h5>Made with love</h5>
                    <h2>Delish Pizza Deals</h2>
                </div>
                <div class="riga">
                    <div class="l-col">
                        <h2>02</h2>
                        <h3>NOV</h3>
                    </div>
                    <div class="r-col">
                        <h3>Traditional Neapolitan pies in kyoto</h3>
                        <h3>Pizza mercato</h3>
                        <h5><span><i class="fas fa-map-marker-alt"></i></span> 204 E. Pizzetta Tommaso</h5>
                    </div>
                </div>
                <div class="riga">
                    <div class="l-col">
                        <h2>02</h2>
                        <h3>NOV</h3>
                    </div>
                    <div class="r-col">
                        <h3>Traditional Neapolitan pies in kyoto</h3>
                        <h3>Pizza mercato</h3>
                        <h5><span><i class="fas fa-map-marker-alt"></i></span> 204 E. Pizzetta Tommaso</h5>
                    </div>
                </div>
                <div class="riga">
                    <div class="l-col">
                        <h2>02</h2>
                        <h3>NOV</h3>
                    </div>
                    <div class="r-col">
                        <h3>Traditional Neapolitan pies in kyoto</h3>
                        <h3>Pizza mercato</h3>
                        <h5><span><i class="fas fa-map-marker-alt"></i></span> 204 E. Pizzetta Tommaso</h5>
                    </div>
                </div>
            </div>
            <div class="right-column col-lg-6 col-md-12">
                <img src="../../../assets/Img/h3-img-5a.jpg" alt="">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name:"Section8"
}
</script>

<style lang="scss" scoped>
    #sezione-8 {
        padding: 0;

        .right-column>img {
            width: 100%;
        }
        .left-column {
            align-self: flex-start;
            background-color: black;
            padding: 100px;
            color: white;
            h2,h3 {
                    text-transform: uppercase;

                }
            .title {
                margin-bottom: 30px;
                h5 {
                    color: #Ab4027;
                    text-transform: uppercase;
                    font-size: 11px;
                    
                }

                h2 {
                    text-transform: uppercase;

                }
            }
            .riga {
                display: flex;
                margin: 25px 0px;
                border-bottom: 1px dotted #B7903C ;
                .l-col {
                    // width: 20%;

                    h2 {
                        font-size: 45px;
                        color: #Ab4027;
                        font-weight: bold;

                    }
                }
                .r-col {
                        margin-left: 50px;

                    h5 {
                        margin-top: 20px;
                        color: #Ab4027;
                        font-size: 15px;
                        cursor: pointer;

                        &:hover {
                            text-decoration: underline;
                        }
                    }
                }
            }
        }
    }
</style>