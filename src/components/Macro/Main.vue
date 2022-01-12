<template>
  <div id="Main">
    <Section1/>
    <Section2/>
    <Section3/>
    <Section4/>
    <Section5/>
    <Section6/>




  </div>
</template>

<script>
import Section1 from "../Sections/main/Section1.vue"
import Section2 from "../Sections/main/Section2.vue"
import Section3 from "../Sections/main/Section3.vue"
import Section4 from "../Sections/main/Section4.vue"
import Section5 from "../Sections/main/Section5.vue"
import Section6 from "../Sections/main/Section6.vue"



export default {
    name:"Main",
    components: {
      Section1,
      Section2,
      Section3,
      Section4,
      Section5,
      Section6,

    }
}
</script>

<style>

</style>