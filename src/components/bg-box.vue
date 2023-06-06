<template>
    <div class="animate-circle-background">
        <div></div>
        <div></div>
        <div></div>
        <div></div>
        <div></div>
        <div></div>
        <div></div>
        <div></div>
        <div></div>
        <div></div>

        <div></div>
        <div></div>
        <div></div>
        <div></div>
        <div></div>
    </div>
</template>

<script setup lang="ts">

</script>

<style>
.animate-circle-background{
    position: absolute; 
    top: 0;
    left: 0;
    height: 100%;
    width: 100%;
    overflow: hidden;
    z-index: 6;
}
.animate-circle-background div{
    position: absolute;
    display: block;
    width: 20px;
    height: 20px;
    background: rgba(0, 173, 181, 0.5);
    bottom: -150px;
    transition: background .5s linear;
    animation: animate-circle-background 25s  linear infinite;
}
.animate-circle-background div:hover{
    background: rgba(0, 173, 181, 1);
    transition: all .5s linear;
}
.animate-circle-background div:nth-child(1){
    left: 25%;  
    width: 80px;
    height: 80px;
    animation-delay: 0;
}   
.animate-circle-background div:nth-child(2){
    left: 10%;  
    width: 20px;
    height: 20px;
    animation-delay: 2s;
    animation-duration: 12s;
}   
.animate-circle-background div:nth-child(3){
    left: 70%;  
    width: 20px;
    height: 20px;
    animation-delay: 4s;
}   
.animate-circle-background div:nth-child(4){
    left: 40%;  
    width: 50px;
    height: 50px;
    animation-delay: 0s;
    animation-duration: 18s;
}   
.animate-circle-background div:nth-child(5){
    left: 65%;  
    width: 20px;
    height: 20px;
    animation-delay: 0s;
}   
.animate-circle-background div:nth-child(6){
    left: 75%;  
    width: 110px;
    height: 110px;
    animation-delay: 3s;
}   
.animate-circle-background div:nth-child(7){
    left: 35%;  
    width: 150px;
    height: 150px;
    animation-delay: 7s;
}   
.animate-circle-background div:nth-child(8){
    left: 50%;  
    width: 25px;
    height: 25px;
    animation-delay: 15s;
    animation-duration: 45s;
}   
.animate-circle-background div:nth-child(9){
    left: 20%;  
    width: 15px;
    height: 15  px;
    animation-delay: 2s;
    animation-duration: 35s;
}   
.animate-circle-background div:nth-child(10){
    left: 85%;  
    width: 150px;
    height: 150px;
    animation-delay: 0s;
    animation-duration: 11s;
}

.animate-circle-background div:nth-child(11){
    left: 5%;  
    width: 70px;
    height: 70px;
    animation-delay: 0s;
    animation-duration: 30s;
}  
.animate-circle-background div:nth-child(12){
    left: 40%;  
    width: 40px;
    height: 40px;
    animation-delay: 2s;
    animation-duration: 20s;
}  
.animate-circle-background div:nth-child(13){
    left: 70%;  
    width: 70px;
    height: 70px;
    animation-delay: 1s;
    animation-duration: 15s;
}  
.animate-circle-background div:nth-child(14){
    left: 30%;  
    width: 30px;
    height: 30px;
    animation-delay: 4s;
    animation-duration: 15s;
}  
.animate-circle-background div:nth-child(15){
    left: 90%;  
    width: 30px;
    height: 30px;
    animation-delay: 4s;
    animation-duration: 15s;
}  

@keyframes animate-circle-background {
    0%{
        opacity: 1;
        border-radius: 0;
        transform: translateY(0) rotate(0deg);
    }
    100%{
        opacity: 0;
        border-radius: 50%;
        transform: translateY(-1000px) rotate(720deg);
    }
}
</style>