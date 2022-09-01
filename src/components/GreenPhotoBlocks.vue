<template>
    <div id="GPBlocks">
        <div class="container">
            <div class="info-block block">
                
                    <div class="qwerty">Фамилия</div>
                    <div class="qwe">Мамай</div>

                    <div class="qwerty">Имя и отчество</div>
                    <div class="qwe">Станиславаленина Владимировна</div>

                    <div class="qwerty">Номер полиса выдан заведомо ложный</div>
                    <div class="qwe">01354879</div>

                    <div class="qwerty">Дата рождения</div>
                    <div class="qwe">01.12.1976</div>

                    <div class="qwerty">Телефон</div>
                    <div class="qwe">+79254218069</div>
 
            </div>
            <div class="green-little block">Понятие модернизации понимает механизм власти</div>
            <div class="yacht-little">
                <div class="yacht"></div>
                <div class="warning-round">!</div>
            </div>
            
            
                
                
            </div>
            
    </div>
    
    
  </template>
  
  <script>
  export default {
    name: 'GPBlock',
    
  }
  </script>
  
  
  <style scoped>
.container {
    margin-top: 10px;
  color: #000;
  display: grid;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 1fr 1fr;
  grid-auto-columns: 1fr;
  gap: 10px 10px;
  grid-auto-flow: row;
  grid-template-areas:
    "green-little info-block info-block"
    "yacht-little info-block info-block";
  
}

.green-little{
    padding: 15px;
    font-size: 14px;
    display: flex;
    flex-direction: column-reverse;
}

.info-block { 
    font-size: 14px;
    display: grid;
    grid-template-columns: 1fr auto;
    grid-template-rows: 15px 15px 15px 15px 15px;
    
    grid-area: info-block;
    gap: 50px;
    background: #E3EBD3;
    aspect-ratio: 1/1;
    
    
    padding: 20px;
    font-size: 14px;
    overflow: hidden;
}

.qwerty{
    
    text-align: start;
    position: relative;
    
    
}
.qwerty::after{
    content: '';
    border: 1px dashed #000000;
    transform: rotate(180deg);
    position: absolute;
    bottom: 0;
    width: 100%;
    
}

.qwe{
    
    text-align: end;

}


.info-block p{
    margin: 0;
    
}



.green-little { grid-area: green-little;background: #E3EBD3; }

.yacht-little { 
    grid-area: yacht-little; 
    position: relative; 
    display: flex;
    justify-content: center;
    align-items:center ;
}

.yacht{
    
    
    background: url(../assets/yacht.png);
    background-size: cover;
    position: absolute;
    width: 100%;
    height: 100%;
}

.yacht-little:hover .yacht{
    filter: blur(10px);
}



.warning-round {
    aspect-ratio: 1/1;
    position: absolute;
    visibility: hidden;
    width: 50px;
    height: 50px;
    color: rgb(255, 0, 0);
    font-size: 30px;
    border-radius: 50%;
    line-height: 50px;
    text-align: center;
    background: #fff;

     
}

.yacht-little:hover .warning-round{
    visibility: visible;
    
}



  </style>
  