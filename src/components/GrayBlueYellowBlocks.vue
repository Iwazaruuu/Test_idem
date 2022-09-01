<template>
    <div id="GBYBlocks">
        <div class="container">
            <div class="Gray-big block">Конформизм</div>
            <div class="Gray-little-1 block">Наши сотрудники</div>
            <div class="Gray-little-2 block">Просветляет понимающий тест</div>
            <div class="Blue-little block">Интроекция</div>
            <div class="Yellow-little block">Наши сотрудники</div>
        </div>
    </div>
    
  </template>
  
  <script>
  export default {
    name: 'GBYBlock',
    
  }
  </script>
  
  
<style scoped>
    .container {  
        margin-top: 10px;
        display: grid;
        grid-template-columns: 1fr 1fr 1fr;
        grid-template-rows: 1fr 1fr;
        grid-auto-columns: 1fr;
        gap: 10px 10px;
        grid-auto-flow: row;
        grid-template-areas:
            "Gray-little-1 Gray-little-2 Blue-little"
            "Gray-big Gray-big Yellow-little";
        }
    .block{
        height: 155px;
        padding: 15px;
        display: flex;
        flex-direction: column-reverse;
        font-size: 14px;
    }
    .Gray-big { grid-area: Gray-big; background: #E8EBED;}

    .Gray-little-1 { grid-area: Gray-little-1; background: #E8EBED;}

    .Gray-little-2 { grid-area: Gray-little-2; background: #E8EBED;}

    .Blue-little { grid-area: Blue-little; background: #90BCE8;}

    .Yellow-little { grid-area: Yellow-little; background: #FEBF26;}
    
    @media screen and (max-width: 480px){
        .container {  
        
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-template-rows: 1fr 1fr 1fr;
        grid-auto-columns: 1fr;
        gap: 10px 10px;
        grid-auto-flow: row;
        grid-template-areas:
            "Gray-little-1 Gray-little-2"
            "Gray-big Gray-big"
            "Blue-little Yellow-little";
        }
        
    }
</style>
  