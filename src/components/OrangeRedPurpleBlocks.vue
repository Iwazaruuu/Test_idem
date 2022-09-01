<template>
    <div id="GBYBlocks">
        <div class="container">
            <div class="Orange-big block">Однако</div>
            <div class="Orange-little-1 block">Лидерство</div>
            <div class="Orange-little-2 block">Точка перегиба</div>
            <div class="Red-little block">Невероятный гений</div>
            <div class="Purple-little block">Длина вектора</div>
        </div>
    </div>
    
  </template>
  
  <script>
  export default {
    name: 'ORPBlock',
    
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
            "Orange-little-1 Orange-big Orange-big"
            "Red-little Orange-little-2 Purple-little";
        }
    .block{
        height: 155px;
        padding: 15px;
        display: flex;
        flex-direction: column-reverse;
        font-size: 14px;
    }
    .Orange-big { grid-area: Orange-big; background: #FFAA87;}

    .Orange-little-1 { grid-area: Orange-little-1; background: #FFAA87;}

    .Orange-little-2 { grid-area: Orange-little-2; background: #FFAA87;}

    .Red-little { grid-area: Red-little; background: #F55E62;}

    .Purple-little { grid-area: Purple-little; background: #C7ABD4;}
    
    @media screen and (max-width: 480px){
        .container{
        display: grid;
        grid-template-columns: 1fr 1fr;
        grid-template-rows: 1fr 1fr 1fr;
        grid-auto-columns: 1fr;
        gap: 10px 10px;
        grid-auto-flow: row;
        grid-template-areas:
            "Orange-big Orange-big"
            "Orange-little-2 Purple-little"
            "Orange-little-1 Red-little";
        }
    }
</style>
  