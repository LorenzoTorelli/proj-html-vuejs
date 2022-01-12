<template>
    <div id="section-2" >
        <!-- <img src="../../../assets/svg/svg-6.svg" alt=""> -->
       <div class="column">
            <div class="prev" @click="prevImg()">
                <p>prev</p>
            </div>
        </div>
        <div class="header-container central">
            <h4>" {{mainSlider[actual].first}} "</h4>
            <h5>{{mainSlider[actual].second}}</h5>
            <div class="point-container">
                <div class="point" :class="actual == 0 ? 'point-colored' : ''" @click="actual = 0"></div>
                <div class="point" :class="actual == 1 ? 'point-colored' : ''" @click="actual = 1"></div>
                <div class="point" :class="actual == 2 ? 'point-colored' : ''" @click="actual = 2"></div>

            </div>
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
    name: "Section2",
    data() {
        return {
            actual: 0,
            mainSlider: [
                {
                    first:"Lorem ipsum, dolor sit amet consectetur adipisicing elit. Fugiat soluta asperiores nostrum, minima assumenda officia voluptatem eaque nulla",
                    second: "Lorem ipsum, dolor sit amet consectetur "
                },
                {
                    first:"minima assumenda officia voluptatem eaque nulla fugit culpa accusamus aperiam voluptatibus quia ab. Iste ipsum inventore beatae non!",
                    second: "Lorem ipsum, dolor sit amet consectetur "
                },
                                {
                    first:"minima assumenda officia voluptatem eaque nulla dolor sit amet consecteturab. Iste ipsum inventore beatae non!",
                    second: "Lorem ipsum, dolor sit amet consectetur "
                },

            ]
        }
    },
        methods: {
            nextImg: function() {
                if (this.actual == this.mainSlider.length-1) {
                    this.actual = 0;
                }
                else{
                    this.actual++;
                }

            },
            prevImg: function() {
                if (this.actual == 0) {
                    this.actual = this.mainSlider.length-1;
                }
                else{
                    this.actual--;
                }
            },
        }
}
</script>

<style lang="scss" scoped>
    #section-2 {
        margin: 150px 0px;
        display: flex;

        .central {
            display: flex;
            flex-direction: column;
            width: 50%;

            h4 {
                font-size: 25px;
                text-align: center;
                margin-bottom:30px ;
                text-transform: uppercase;
                font-weight: bold;
            }

            h5 {
                color: #d2401e;
                font-size: 15px;
                text-transform: uppercase;

            }
            .point-container {
                display: flex;

                .point {
                    height: 8px;
                    width: 8px;
                    margin: 5px;
                    border-radius: 50%;
                    background-color: lightgray;
}
                .point-colored {
                    background-color: #B7903C;
                }
            }
        }
    }
</style>