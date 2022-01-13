<template>
  <div id="Main">
    <Section1/>
    <Section2/>
    <Section3/>
    <Section4/>
    <Section5/>
    <Section6/>
    <Section7/>
    <Section8/>
    <Section9/>

    <div id="Up" @click="scroll()">
      <img src="../../assets/svg/svg-4.svg" alt="">
    </div>
  </div>
</template>

<script>
import Section1 from "../Sections/main/Section1.vue"
import Section2 from "../Sections/main/Section2.vue"
import Section3 from "../Sections/main/Section3.vue"
import Section4 from "../Sections/main/Section4.vue"
import Section5 from "../Sections/main/Section5.vue"
import Section6 from "../Sections/main/Section6.vue"
import Section7 from "../Sections/main/Section7.vue"
import Section8 from "../Sections/main/Section8.vue"
import Section9 from "../Sections/main/Section9.vue"





export default {
    name:"Main",
    components: {
      Section1,
      Section2,
      Section3,
      Section4,
      Section5,
      Section6,
      Section7,
      Section8,
      Section9,
    }, 
    methods: {
      scroll() {
        window.scrollTo({
          top: 0,
          left: 0,
          behavior: 'smooth',
        });
      }
    } 
}
</script>

<style lang="scss" scoped>
  #Up {
    position: fixed;
    bottom: 20px;
    right: 20px;
    padding: 5px 10px;
    border-radius: 50%;
    background-color: white;
    cursor: pointer;
  }
</style>