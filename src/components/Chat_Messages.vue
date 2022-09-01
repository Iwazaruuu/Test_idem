<template lang="">
    <div id="chat_messages">
        <div class="chat_mes">
            <div class="container">
                <div class="avatar_1"><img src="../assets/avatar.jpg" alt=""></div>
                <div class="meassages msg_1">Это означает, что в Вашем доме, офисе, кабинете, мастерской хранятся ценности бóльшие, чем просто деньги или драгоценности, - культурные ценности. 
                    Произведения искусства, антиквариат, иные предметы коллекционирования – все это имущество, 
                    безусловно высокая стоимость которого. </div>
                <div class="avatar_2"></div>
            </div>
            <div class="container">
                <div class="avatar_1"></div>
                <div class="meassages msg_2">Это означает,</div>
                <div class="avatar_2"><img src="../assets/avatar.jpg" alt=""></div>
            </div>
            <div class="container mes_3">
                <div class="avatar_1"><img src="../assets/avatar.jpg" alt=""></div>
                <div class="meassages msg_3">доме, офисе, кабинете, мастерской</div>
                <div class="avatar_2"></div>
            </div>

            <div class="date" style="display:flex;">
                <hr class="line line-1"> <p>21 октября 2017</p> <hr class="line line-2">
            </div>
            <div class="container">
                <div class="avatar_1"></div>
                <div class="meassages msg_2">Это означает,</div>
                <div class="avatar_2"><img src="../assets/avatar.jpg" alt=""></div>
            </div>
            <div class="container mes_3">
                <div class="avatar_1"><img src="../assets/avatar.jpg" alt=""></div>
                <div class="meassages msg_3">доме, офисе, кабинете, мастерской</div>
                <div class="avatar_2"></div>
            </div>
        </div>

        <div class="input_messages">
            <textarea class="textarea" placeholder="Cowkeifjowefwehifuhqiwuehfqwef wef"></textarea>
        </div>
        <button class="button_submit">Отправить</button>
    </div>
</template>
<script>
export default {
    name:'chat_messages'
}
</script>
<style scoped>
    #chat_messages{
        font-size: 14px;
        
    }
    .chat_mes{
        overflow-y: scroll;
        overflow-x: none;
        z-index: 40;
        
    }
    .container { 
        margin: 30px 0 20px 0;
        display: grid;
        grid-template-columns: auto 1fr auto;
        grid-template-rows: 1fr 1fr;
        grid-auto-columns: 1fr;
        gap: 0px 10px;
        grid-auto-flow: row;
        grid-template-areas:
            "avatar_1 meassages avatar_2"
            "avatar_1 meassages avatar_2";
        }

    .avatar_1 { grid-area: avatar_1; width: 47px; }
    .avatar_1 img{width: 47px; clip-path: polygon(50% 0, 100% 38%, 82% 100%, 18% 100%, 0% 38%);}
    .meassages { grid-area: meassages; background: #F1F3F5; padding: 15px; width: 440px; border-radius: 5px;}
    .msg_3{width: 250px;}
    .msg_2{justify-self: end; width: auto;}
    .avatar_2 { grid-area: avatar_2; }
    .avatar_2 img{width: 47px; clip-path: polygon(50% 0, 100% 38%, 82% 100%, 18% 100%, 0% 38%);}
    
    .date{
        position: relative;
        justify-content: center;
    }
    .date p{
        margin: 0;
        z-index: 11;
        font-family: 'Roboto';
        font-style: normal;
        font-weight: 400;
        font-size: 14px;
        
    }
    .line{
        position: absolute;
        width: 45%;

    }
    .line-1{
        left:-4%;
        z-index: 10;
    }
    .line-2{
        right:0%;
        z-index: 10;
        width: 40%;
    }



    .input_messages{
        padding: 20px 0 0 0 ;
        border-top: 1px solid #fff;
    }
    .textarea{
        box-sizing: border-box;
        width: 590px;
        height: 129px;
        border: 1px solid #DBDBDB;
        border-radius: 4px;

    }
    .textarea:focus{
        outline: none;
        border: none;
        border: 1px solid #DBDBDB;
    }
    .textarea:hover{
        outline: none;
        border: none;
        border: 1px solid #DBDBDB;
    }

    .button_submit{
        background: #0F54B9;
        box-shadow: 0px 4px 6px rgba(15, 84, 185, 0.3);
        border-radius: 21px;
        border: none;
        padding: 10px 20px;
        font-size: 16px;
        color: #fff;
        font-weight: 400;
        margin: 30px 0;
        cursor: pointer;
    }
</style>