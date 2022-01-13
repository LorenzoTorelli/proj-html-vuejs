<template>
  <div id="header">
       
        <HeaderSmart v-if="medium"/>
        <HeaderDesktop v-else/>
        <Jumbotron/>
    </div>
</template>

<script>
import HeaderDesktop from "../Sections/header/HeaderDesktop.vue"
import HeaderSmart from "../Sections/header/HeaderSmart.vue"
import Jumbotron from "../Sections/header/Jumbotron.vue"

export default {
    name:"Header",
    components: {
        HeaderDesktop, 
        Jumbotron,
        HeaderSmart,
    },
    data() {
        return {
            medium: false
        }
    },
    created() {
         window.addEventListener("resize", () => {
             if(window.innerWidth < 990) {
                 this.medium= true;
             }
             else {
                 this.medium = false;
             }
         });
    },
    
}
    

</script>

<style lang="scss" scoped>
    #header {
        // height: 500px;
        width: 100%;
        background-color: black;

       

    }
</style>