<template>
  <div id="app">
    
    <div id="content">
      <router-view/>
    </div>
    
    
  </div>
</template>
<script>
import Navbar from '@/components/Navbar.vue'
import FooterS from '@/components/Footer.vue'
export default {
  components:{
    Navbar,
    FooterS
  }
}
</script>
<style scoped>
#app{
  height: 100%;
  margin: 0;
  font-family: Roboto;
  font-weight: 400;
}



</style>
