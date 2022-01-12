<template>
    <div id="sezione-8">
        <div class="left-column">
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
                    <h5>204 E. Pizzetta Tommaso</h5>
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
                    <h5>204 E. Pizzetta Tommaso</h5>

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
                    <h5>204 E. Pizzetta Tommaso</h5>

                </div>
            </div>
        </div>
        <div class="right-column">
            <img src="../../../assets/Img/h3-img-5a.jpg" alt="">
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
        display: flex;
        margin: 20px 0px;
        .left-column, .right-column {
            width: 50%;
            img{
                width: 100%;
            }
        }

        .left-column {
            align-self: flex-start;
            // justify-self: center;
            background-color: black;
            padding: 150px;
            color: white;
            .title {
                margin-bottom: 30px;

            }
            .riga {
                display: flex;
                width: 100%;
                margin-bottom: 30px;
                padding-bottom: 30px;
                border-bottom: 1px dotted yellow ;
                .l-col {
                    width: 20%;

                    h2 {
                        font-size: 45px;
                    }
                }
                .r-col {
                    h5 {
                        margin-top: 20px;
                        color: red;
                    }
                }
            }
        }
    }
</style>