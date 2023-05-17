<template>
    <h1>Whatsapp 3C+</h1>
 <div class="div-pagina">
    </div>
    <img class="border2" src="../assets/teste.png" alt="border2">
    <img class="imgHome" src="../assets/imgHome.png" alt="imgHome">
    <semVip/>
</template>

<script>

import semVip from './semVip.vue';

export default{
    name: 'my-pagina',
    data(){

    },
    
    components:{
        semVip

    },
}
</script>

<style scoped>

*{
top: 0px;
right: 0px;
bottom: 0px;
left: 0px;

}

.border2{
    position: absolute;
    width: 1600px;
    height: 79px;
    left: 320px;
    top: 882px;
}
.imgHome{

    position: absolute;
    width: 952px;
    height: 653.16px;
    left: 968px;
    top: 152px;



}



.div-pagina{
    /* Auto layout */
    background-color:  #F5F5F5;
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    padding: 0px;
    gap: 32px;

}

.Texts{
/* Auto layout */

    display: flex;
    flex-direction: column;
    align-items: flex-start;
    padding: 0px;
    gap: 12px;

    width: 433px;
    height: 132px;



    /* Inside auto layout */

    flex: none;
    order: 1;
    flex-grow: 0;
}
h1{
    position: relative;
    height: 40px;
    width: 288px;
    left: 388px;
    right: 12px;
    top: 40px;
    font-family: 'Random Grotesque Standard Semibold';
    font-style: normal;
    font-weight: 600;
    font-size: 32px;
    line-height: 40px;
    letter-spacing: -0.01em;
    color: #12263F;
}








</style>