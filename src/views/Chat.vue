<template>
  <button @click="$router.push('/')" class="chat_button">Перейти на страницу вёрстки</button>
  <div id="chat">
    <ChatMsg/>
  </div>
</template>

<script>
import ChatMsg from '@/components/Chat_Messages.vue'
export default {
  name: 'Chat',
  components: {
    ChatMsg
  }
}
</script>

<style scoped>
  #chat{
    width: 651px;
    height: 757px;
    background: url(../assets/chat_bg.png);
    margin: auto;
    padding: 40px 30px;
  }
  
  .chat_button{
  margin: 10px 0 0 0;
  padding: 10px;
  border: none;
  cursor: pointer;

}
</style>
