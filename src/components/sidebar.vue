<template>
    <div class="sidebar">
        <div class="sidebar1">
            <img alt="3C logo" src="../assets/logo.png">
        </div>
        <img class="border" src="../assets/border.png" alt="border">
        <div class="receptivo">
        
            <div class="whatsapp">
                 <img alt="wpp logo" src="../assets/wpp.png"> 
            <p>Whatsapp</p>
            </div>
        </div>
    </div>
        
    </template>
    
    <script>
    export default{
        name: 'my-sidebar',
    }
    
    </script>
    
    
    <style scoped>
    
    *{
    top: 0px;
    right: 0px;
    bottom: 0px;
    left: 0px;
    
    }
    
    
    .border{
        position: absolute;
        width: 10px;
        height: 40px;
        top: 148px;
    
    
    }
    
    
    
    
    .sidebar {
    background:white;
    
    /* Menu lateral */
    position: absolute;
    left: 0px;
    right: 83.33%;
    top: 0%;
    bottom: 0%;
    
    
    }
    
    
    
    .sidebar1 {
        position: absolute;
        width: 92.09px;
        height: 50px;
        left: 105px;
        top: 44px;
    
    }
    
    .receptivo{
        position: absolute;
        width: 196px;
        height: 22px;
        left: 10px;
        top: 122px;
    
    }
    
    .whatsapp{
        background-color: white;
        display: flex;
        flex-direction: row;
        align-items: center;
        padding: 20px;
        gap: 10px;
    
    }
    
    .sidebar2 {
       
        background-color: white;
        width: 20px;
        height: 20px;
    
    
        /* Inside auto layout */
    
        flex: none;
        order: 0;
        flex-grow: 0;
    }
    .textWpp{
    
        width: 78px;
        height: 22px;
        font-family: 'Inter';
        font-style: normal;
        font-weight: 400;
        font-size: 15px;
        line-height: 22px;
        letter-spacing: -0.01em;
        color: #1B1B2B;
        flex: none;
        order: 1;
        flex-grow: 0;
    }
    
    
    
    </style>