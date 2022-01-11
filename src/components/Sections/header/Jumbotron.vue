<template>
    <div id="jumbotron">
        <div class="column">
            <div class="prev" @click="prevImg()">
                <p>prev</p>
            </div>
        </div>
        <div class="header-container">
            <img class="front" :src="require( `../../../assets/Img/${this.jumbo[actual].front}.png`)" alt="">
            <img class="back" :src="require( `../../../assets/Img/${this.jumbo[actual].back}.png`)" alt="">
        </div>
        <div class="column">
            <div class="next" @click="nextImg()">
                <p>next</p>
            </div>
        </div>

        
    </div>
</template>

<script>
export default {
    name:"Jumbotron",
    data() {
        return {
            actual: 0,
            jumbo: [
                {
                    front: "h3-rev-img-6",
                    back: "h3-rev-img-5",
                    "num":1,
                },
                {
                    front: "h3-rev-img-4",
                    back:"h3-rev-img-3",
                    "num":2,
                },
                {
                    front: "h3-rev-img-2",
                    back:"h3-rev-img-1",
                    "num":3,
                }
            ]
        }
    },
    methods: {
            nextImg: function() {
                if (this.actual == this.jumbo.length-1) {
                    this.actual = 0;
                }
                else{
                    this.actual++;
                }

            },
            prevImg: function() {
                if (this.actual == 0) {
                    this.actual = this.jumbo.length-1;
                }
                else{
                    this.actual--;
                }
            },
        }
}
</script>

<style lang="scss" scoped>
    #jumbotron {
        height: 500px;
        width: 100%;
        // background-image: url("../../assets/Img/h3-testimonials-bckgrnd.jpg");
        // filter: 1;
        display: flex;

        .header-container {
            height: 100%;
            position: relative;

            .front {
                position: absolute;
                // height: 100px;
                width: 250px;
                // top: 0;
            }
        }

        .column {
            width: 15%;
            position: relative;
            height: 100%;
            .next, .prev {
                position: absolute;
                // align-self: center;
                width: 25px;
                height: 50px;
                top: 40%;
                background-color: white;
                cursor: pointer;

            }
            .next {
                right: 0;
                border-radius: 50px 0px 0px 50px;
                p {
                    writing-mode: vertical-rl; 
                    margin-top:10px ;
                    margin-left: 3px;
                    color:#D2401E;
                }
            }
            .prev {
                border-radius: 0px 50px 50px 0px;
                p {
                    // text-orientation: mixed;
                    writing-mode: vertical-rl; 
                    margin-top:10px ;
                    margin-left: 3px;
                    color:#D2401E;
                }
            }
        }
    }
</style>