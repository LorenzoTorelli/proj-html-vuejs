<template>
  <div id="Main">
    <Section1/>
    <Section2/>

  </div>
</template>

<script>
import Section1 from "../Sections/main/Section1.vue"
import Section2 from "../Sections/main/Section2.vue"
export default {
    name:"Main",
    components: {
      Section1,
      Section2
    }
}
</script>

<style>

</style>