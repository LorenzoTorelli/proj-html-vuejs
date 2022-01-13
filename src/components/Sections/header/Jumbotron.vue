<template>
    <div id="jumbotron" >

        <div class="container-fluid">
            <div class="row">
               <div class="column-1 col-1">
                    <div class="prev" @click="prevImg()">
                        <p>prev</p>
                    </div>
                </div>
                <div class="central col-10">
                    <img class="front" :src="require( `../../../assets/Img/${this.jumbo[actual].front}.png`)" alt="">
                    <img class="back" :src="require( `../../../assets/Img/${this.jumbo[actual].back}.png`)" alt="">
                </div>
                <div class="column-2 col-1">
                    <div class="next" @click="nextImg()">
                        <p>next</p>
                    </div>
                </div>
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
                },
                {
                    front: "h3-rev-img-4",
                    back:"h3-rev-img-3",
                },
                {
                    front: "h3-rev-img-2",
                    back:"h3-rev-img-1",
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
        height: 40vw;
        max-height: 600px;
        min-height: 300px;
        display: flex;
        align-items: center;
        padding: 25px 0px 50px;
        .central {
            position: relative;
            
            .back {
                width: 80%;
            }
            .front {
                position: absolute;
                width: 20%;
            }
        }
       
        

 
    }
</style>