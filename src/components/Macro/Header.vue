<template>
  <div id="header">
    <div class="header-container">

        <!-- settore sinistra  -->
        <div class="sector">
            <div class="btn-container">
                <div class="btn">
                    Order Online
                </div>
            </div>
            <ul class="first-bar">
                <!-- <img src= alt=""> -->
                <HeaderComponent v-for='(el,index) in navBarFirst' :key='index'
                    :name= "el.name"
                    :logo= "el.logo"
                    :link= "el.link"
                />
            </ul>
        </div>

        <!-- logo  -->
        <div class="logo">
            <img src="../../assets/Img/h5-logo-divided-header.png" alt="logo">
        </div>

        <!-- settore destra  -->
        <div class="sector">
            <ul class="first-bar">
                <HeaderComponent v-for='(el,index) in navBarSecond' :key='index'
                    :name= "el.name"
                    :logo= "el.logo"
                    :link= "el.link"
                />
            </ul>
            <ul class="first-bar">
                <HeaderComponent v-for='(el,index) in navBarLast' :key='index'
                    :name= "el.name"
                    :logo= "el.logo"
                    :link= "el.link"
                />
            </ul>
        </div>
    </div>
    <Jumbotron/>
  </div>
</template>

<script>
import HeaderComponent from "../Sections/header/HeaderComponent.vue"
import Jumbotron from "../Sections/header/Jumbotron.vue"
export default {
    name:"Header",
    components: {
        HeaderComponent, 
        Jumbotron,
    },
    data() {
        return {
            navBarFirst: [
                {
                    "name":"home",
                    "logo": "svg-0",
                    "link":"#"
                },
                    {
                    "name":"pages",
                    "logo": "",
                    "link":"#"
                },
                {
                    "name":"menu",
                    "logo": "",
                    "link":"#"
                }
            ], 
            navBarSecond: [
                  {
                    "name":"event",
                    "logo": "",
                    "link":"#"
                },
                    {
                    "name":"blog",
                    "logo": "",
                    "link":"#"
                },
                {
                    "name":"landing",
                    "logo": "",
                    "link":"#"
                }
            ],
            navBarLast: [
                  {
                    "name":"cart",
                    "logo": "svg-1",
                    "link":"#"
                },
                    {
                    "name":"search",
                    "logo": "",
                    "link":"#"
                },
               
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    #header {
        // height: 500px;
        width: 100%;
        background-color: black;

        .sector {
            width: 40%;
            display: flex;
            justify-content: space-between;

            .btn-container {
                padding: 25px;

            .btn {
                background-color: #D2401E;
                padding: 15px 20px;
                text-transform: uppercase;
                color: #FFFFFF;

            }
            }
            .first-bar{
                display: flex;
                align-items: center;
                // background-color: green;
            }
            .first-bar:nth-child(1) {
                margin-left: -7px;
                // background-color: red;
            }
        }
        
        .logo {
            width: 10%;
            padding: 10px 0px;
            // background-color: red;
            img {
                // height: 80px;
                width: 100%;
                object-fit: cover;

            }
        }

    }
</style>