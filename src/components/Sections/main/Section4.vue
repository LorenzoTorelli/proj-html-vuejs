<template>
    <div id="section-4">
        <div class="riga-1">
            <div class="col-1"></div>
            <div class="col-2"></div>
            <div class="col-3"></div>
        </div>

        <div class="riga-2">
            <div class="col-1"></div>
            <div class="col-2"></div>
            <div class="col-3"></div>
        </div>

         <div class="riga-3">
            <div class="col-1"></div>
            <div class="col-2"></div>
            <div class="col-3"></div>
        </div>

        <div class="text">
            <h2>Go Ahead an build your own pizza we won't judge!</h2>
        </div>
        
    </div>
</template>

<script>
export default {
    name:"Section4"
}
</script>

<style lang="scss" scoped>
    #section-4 {
        width: 100%;
        height: 600px;
        margin: 10px 0px ;
        position: relative;

        .col-1, .col-2, .col-3 {
            background-image: url("../../../assets/Img/h3-background-img.jpg");
            // border: 1px solid white;
            background-repeat:no-repeat;

            // background-color: red;

        }
        .col-1, .col-3 {
            height: 100%;
            width: 5%;
        }

        .col-2 {
            width: 90%;
            height: 100%;

        }
        .riga-1, .riga-2, .riga-3 {
            display: flex;
        }

        .riga-1, .riga-3 {
            height: 20%;
            width: 100%;
        }
        .riga-1 {
            .col-1{
                background-position:right bottom;            
            }
            .col-2{
                background-position:center bottom;            
            }
            .col-3{
                background-position:left bottom;
            }
        }
        .riga-2 {
           height: 60%;
           width: 100%;
            .col-1{
                background-position:right top;
            }
            .col-2{
                background-position:center top;
            }
            .col-3{
                background-position:left top;

            }
        }

        .riga-3 {
            .col-1{
                    background-position:right center;
                }
                .col-2{
                    background-position:center ;
                }
                .col-3{
                    background-position:left center;
                }
        }

        .text {
            position: absolute;
            width: 300px;
            top: 50%;
            left:50%;
            margin-left: 25px;
            transform: translate(-50%, -50%);
            h2 {
                color: white;
                text-transform: uppercase;
                font-size: 45px;
            }
        }
        
    }
</style>
