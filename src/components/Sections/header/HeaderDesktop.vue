<template>
  <div id="header-desktop">
       <div class="container-lg">

            <div class="row">
                <!-- settore sinistra  -->
                <div class="sector-1 col-5">
                    <a href="#section-9" class="my-btn">Order Online</a>
                    <ul class="first-bar">
                        <!-- <img src= alt=""> -->
                        <HeaderComponent v-for='(el,index) in data.navBarFirst' :key='index'
                            :name= "el.name"
                            :logo= "el.logo"
                            :link= "el.link"
                        />
                    </ul>
                </div>
                <!-- logo  -->
                <div class="logo col-2">
                    <img src="../../../assets/Img/h5-logo-divided-header.png" alt="logo">
                </div>
                <!-- settore destra  -->
                <div class="sector-2 col-5">
                    <ul class="first-bar">
                        <HeaderComponent v-for='(el,index) in data.navBarSecond' :key='index'
                            :name= "el.name"
                            :logo= "el.logo"
                            :link= "el.link"
                        />
                    </ul>
                    <ul class="first-bar">
                        <HeaderComponent v-for='(el,index) in data.navBarLast' :key='index'
                            :name= "el.name"
                            :logo= "el.logo"
                            :link= "el.link"
                        />
                    </ul>
                </div>
            </div>
        </div>
  </div>
</template>

<script>
import HeaderComponent from "../header/HeaderComponent.vue"
import data from "../../../share/data"
export default {
    
    name:"HeaderDesktop",
    components: {
        HeaderComponent
    },
    data() {
        return {
            data
        }
    }
}
</script>

<style lang="scss" scoped>
    #header-desktop {
        padding: 20px 0px;
        .sector-1, .sector-2 {
            display: flex;
            align-items: center;
            justify-content: space-around;

            .first-bar {
                display: flex;
            }
        }
        .sector-1 {
            .my-btn {
                margin-top: -15px;
            }
        }
        .sector-2 {
            ul {
                padding: 0;
            }
        }
        .logo {
            img {
                width: 100%;
            }
        }
    }




</style>