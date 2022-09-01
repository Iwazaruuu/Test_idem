<template>
    <div id="Pblocks">
        <div class="container">
            <div class="big-block">Гений непредвзято понимает под собой конфликт. Закон внешнего мира, очевидно, реально подчеркивает аксиоматичный здравый смысл. Культ джайнизма включает в себя поклонение Махавире и другим тиртханкарам, поэтому закон исключённого третьего индуцирует изоморфный ротор.</div>
            <div class="first-little">Чувство однократно</div>
            <div class="second-little">Морено</div>
        </div>
    </div>
    
  </template>
  
  <script>
  export default {
    name: 'PBlock',
    
  }
  </script>
  
  
  <style scoped>
.container { 
  color: #fff;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr;
  grid-auto-columns: 1fr;
  gap: 10px 10px;
  grid-auto-flow: row;
  grid-template-areas:
    "big-block big-block first-little"
    "big-block big-block second-little";
  
}

.big-block { grid-area: big-block;background: #A2A9B7; font-size: 18.11px; padding: 30px 46px 53px 25px; text-align: center; overflow-y: scroll ; ; aspect-ratio: 1/1;}

.first-little { grid-area: first-little;background: #A2A9B7;font-size: 14px; padding:15px; display: flex; flex-direction: column-reverse;}

.second-little { grid-area: second-little;background: #A2A9B7;font-size: 14px; padding: 15px; display: flex; flex-direction: column-reverse;}

@media screen and (max-width: 480px){
    
}
  </style>
  