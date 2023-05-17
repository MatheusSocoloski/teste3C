<template>
    <div>
        <button class="btn2">Quero ter acesso antecipado</button>
    </div>

</template>

<script>


export default{
    name: 'my-btn2',
    }


 


</script>

<style scoped>
.btn2{
    box-sizing: border-box;

/* Auto layout */
    
    flex-direction: row;
    justify-content: center;
    align-items: center;
    padding: 11px 16px;
    gap: 8px;
    background: #3057F2;
    border: 1px solid #3057F2;
    border-radius: 10px;
    flex: none;
    order: 2;
    flex-grow: 0;

    
    position: absolute;
    width: 300px;
    height: 40px;
    right: 36px;
    left: 1000px;
    top: -150px;


    font-family: 'Cerebri Sans Pro';
    font-style: normal;
    font-weight: 500;
    font-size: 16px;
    line-height: 18px;
    color: white;
}




</style>