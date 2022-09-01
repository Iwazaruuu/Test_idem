<template>
  <Navbar/>
  <div id="home">
    
    <button @click="$router.push('Chat')" class="chat_button">Перейти в чат</button>
    <div class="reverse-blocks">
      <PBlock/>
      <GBYBlock/>
    </div>
    <GPBlock class="GPBlock"/>
    <ORPBlock/>
    
  </div>
  <FooterS/>
</template>

<style scoped>
#home{
  margin: 10px 10px;
}
.chat_button{
  margin: 10px 0 0 0;
  padding: 10px;
  border: none;
  cursor: pointer;

}
.reverse-blocks{
  margin: 10px 0 0 0;
  
}

@media screen and (max-width: 480px){
  .reverse-blocks{
  gap:10px;
  display: flex;
  flex-direction: column-reverse;
  margin: 10px 0 0 0;
}
  .GPBlock{
    display: none;
  }
}
</style>


<script>


import PBlock from '@/components/PurpleBlocks.vue'
import GBYBlock from '@/components/GrayBlueYellowBlocks.vue'
import GPBlock from '@/components/GreenPhotoBlocks.vue'
import ORPBlock from '@/components/OrangeRedPurpleBlocks.vue'
import Navbar from '@/components/Navbar.vue'
import FooterS from '@/components/Footer.vue'

export default {
  name: 'Home',
  components: {
    PBlock,
    GBYBlock,
    GPBlock,
    ORPBlock,
    Navbar,
    FooterS
  }
}
</script>
<!-- <div class="button">
      <button @click="$router.push({name: 'chat'})"><span>Перейти на страницу чата</span></button>
    </div> -->