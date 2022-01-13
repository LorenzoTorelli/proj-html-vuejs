<template>
    <div id="header-smart">
        <div class="container-lg">
            <div class="row">
                <div class="col-6">
                    <img src="../../../assets/Img/mobile.png" alt="">
                </div>
                <div class="col-6 second" >
                    <div class="hamb" @click="animationToggle = !animationToggle" :class="{change:animationToggle}">
                        <div class="bar1"></div>
                        <div class="bar2"></div>
                        <div class="bar3"></div>
                    </div>
                    <div class="dropdown" v-show="animationToggle">
                        <ul class="list">
                            <HeaderComponent v-for='(el,index) in data.navBarFirst' :key='index'
                            :name= "el.name"
                            :link= "el.link"
                        />
                        </ul>
                        <ul class="list">
                           <HeaderComponent v-for='(el,index) in data.navBarSecond' :key='index'
                            :name= "el.name"
                            :link= "el.link"
                        />
                        </ul>
                        <ul class="list">
                           <HeaderComponent v-for='(el,index) in data.navBarLast' :key='index'
                            :name= "el.name"
                            :link= "el.link"
                        />
                        </ul>
                         <div class="my-btn">
                            Order Online
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import data from "../../../share/data"
import HeaderComponent from "../header/HeaderComponent.vue"

export default {
    name:"HeaderSmart",
    components: {
        HeaderComponent
    },
     data() {
        return {
            animationToggle: false,
            data

        }   
    },
}
</script>

<style lang="scss" scoped>
    #header-smart {
        padding: 20px 0px;
        .my-btn {
            text-align: center;
        }
        .hamb {
            cursor: pointer;
            float: right;
            margin-right: 35px;
            margin-top: 15px;
            // right: 0;
            .bar1, .bar2, .bar3 {
                width: 35px;
                height: 5px;
                background-color: #B7903C;
                margin: 6px 0;
                transition: 0.4s;

            }
        }

        .change {
            .bar1 {
                -webkit-transform: rotate(-45deg) translate(-9px, 6px);
                transform: rotate(-45deg) translate(-8px, 6px);
            }
            .bar2 {opacity: 0;}

            .bar3 {
                -webkit-transform: rotate(45deg) translate(-8px, -8px);
                transform: rotate(45deg) translate(-8px, -8px);
            }         
        }

        .dropdown {
            position: absolute;
            background-color: black;
            width: 100%;
            left: 0;
            box-shadow: 0 6px 2px -2px balck;
            z-index: 1;
            margin-top: 80px;
            .list {
                margin-top: 20px;
                // border-bottom: 1px dotted #B7903C;
            }
            a {
                text-decoration: none;
                color:black;
            }
            li {
                list-style: none;
            }
            .button {
                margin-top:20px;
                a {
                    color: #2485fd;
                }
            }


        }
    }
</style>