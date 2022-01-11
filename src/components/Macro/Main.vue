<template>
  <div id="Main">
    <Section1/>
    <Section2/>
    <Section3/>

  </div>
</template>

<script>
import Section1 from "../Sections/main/Section1.vue"
import Section2 from "../Sections/main/Section2.vue"
import Section3 from "../Sections/main/Section3.vue"
export default {
    name:"Main",
    components: {
      Section1,
      Section2,
      Section3,
    }
}
</script>

<style>

</style>