<template>
    <section class="relative first">
        <div class="h-[50px] flex bg-transparent">
            <div class="h-full w-[150px] border-b-4 border-r-4 border-[#00ADB5] rounded-br-xl bg-c-222831 flex items-center justify-center z-10">
                <span class="font-bold text-[1.5rem] tracking-wider color-EEEEEE">
                    <span class="color-00ADB5">D</span>o<span class="color-00ADB5">D</span>ong
                </span>
            </div>
            <div class="h-full w-[calc(100%-150px)] bg-transparent z-10">   
                <div class="h-full w-full flex items-center justify-between rounded-t-xl bg-transparent px-[6px]">
                    <div>
                        <navBar/>
                    </div>
                    <div class="flex items-center">
                        <div class="h-full flex mr-0">
                            <a href="dong.asumbra@gmail.com" target="_blank" class="flex social email">
                                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-mail">
                                    <path d="M4 4h16c1.1 0 2 .9 2 2v12c0 1.1-.9 2-2 2H4c-1.1 0-2-.9-2-2V6c0-1.1.9-2 2-2z"></path>
                                    <polyline points="22,6 12,13 2,6"></polyline>
                                </svg>
                                <span>Email</span>
                            </a>
                            <a href="https://github.com/DoDongssss" target="_blank" class="flex social github">
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-github">
                                    <path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path>
                                    </svg>
                                <span>Github</span>
                            </a>
                            <a href="https://www.linkedin.com/in/johnny-asumbra-0b8b5a25a/" class="flex social linkedin">
                                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-linkedin">
                                    <path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"></path>
                                    <rect x="2" y="9" width="4" height="12"></rect>
                                    <circle cx="4" cy="4" r="2"></circle>
                                </svg>
                                <span>Linkedin</span>
                            </a>
                            <a href="https://www.facebook.com/TuDesse/" target="_blank" class="flex social facebook">
                                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-facebook">
                                    <path d="M18 2h-3a5 5 0 0 0-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 0 1 1-1h3z"></path>
                                </svg>
                                <span>Facebook</span>
                            </a>
                            <a href="https://www.instagram.com/asumbra_/" target="_blank"  class="flex social instagram">
                                <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-instagram">
                                    <rect x="2" y="2" width="20" height="20" rx="5" ry="5"></rect>
                                    <path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"></path>
                                    <line x1="17.5" y1="6.5" x2="17.51" y2="6.5"></line></svg>
                                <span>Instagram</span>
                            </a>
                            <a href="https://twitter.com/xchitts" target="_blank" class="flex social twitter"  >
                                <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-twitter">
                                    <path d="M23 3a10.9 10.9 0 0 1-3.14 1.53 4.48 4.48 0 0 0-7.86 3v1A10.66 10.66 0 0 1 3 4s-4 9 5 13a11.64 11.64 0 0 1-7 2c9 5 20 0 20-11.5a4.5 4.5 0 0 0-.08-.83A7.72 7.72 0 0 0 23 3z"></path>
                                </svg>
                                <span>Twitter</span>
                            </a>
                        </div>
                        <div class="h-full flex items-center justify-start rounded-bl-xl">
                            <el-switch
                                v-model="themeSwitch"
                                :loading="switchLoading"
                                :before-change="switchBeforeChange"
                                class="ml-2"
                                style="--el-switch-on-color: #222831; --el-switch-off-color: #ffcc00"
                            />
                        </div>
                    </div>
                </div>
            </div> 
        </div>
        <main class="relative flex h-[calc(100%-50px)] rounded-l-xl bg-transparent color-222831 py-[5rem] pl-[10rem] pr-[5rem] z-10">
            <div class="h-full basis-1/2 flex flex-col items-center justify-center shrink-0">
                <div class="w-full flex items-center justify-between overflow-hidden">
                    <span class="w-[35%] border-b-[2px] border-[#00ADB5] hello-stick-one"></span>
                        <span class="font-bold tracking-[5px] text-sm color-393E46 px-2">HELLO I'M</span>
                    <span class="w-[35%] border-b-[2px] border-[#00ADB5] hello-stick-two"></span>
                </div>  
                <h1 class="font-bold text-[3.4rem] font-rowdie tracking-wider fullname">Johnny A. Asumbra</h1>
                <p class="text-base text-center lg:text-justify color-222831 mt-5 info-msg overflow-hidden">
                    Welcome to my portfolio! I'm a web developer passionate about developing websites. Explore my work, testimonials, and professional background. Let's connect and collaborate on exciting projects. Thank you for visiting!
                </p>
                <div class="w-full flex mt-9"> 
                        <button type="button" class="mr-3 py-[10.5px] px-5 bg-c-00ADB5 rounded-[5px] tracking-wide font-bold text-white">Download CV</button>
                        <button type="button" class="flex py-[10.5px] px-5 rounded-[5px] tracking-wide font-bold text-[#393E46] btn-contact z-20">
                            Contact Me
                            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1" stroke-linecap="round" stroke-linejoin="round" class="feather feather-arrow-right ml-1">
                                <line x1="5" y1="12" x2="19" y2="12"></line>
                                <polyline points="12 5 19 12 12 19"></polyline>
                            </svg>
                        </button>
                </div>
            </div>
            <div class="h-full basis-1/2 flex items-center justify-center shrink">
                <div class="h-[400px] w-[400px] img-wrapper">
                    <img src="../../src/assets/images/ako.jpg" alt="" class="h-full w-full ako-img">
                </div>
            </div>
            <div class="absolute bottom-[-5px] right-[-5px] h-[20px] w-[20px] border-8 border-[#222831] rounded-[50%]">
            </div>
        </main>

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
        </div>

        <!-- <div class="section-cover"></div> -->
    </section>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue'
import navBar from '../../src/components/nav.vue'

export default defineComponent({
    components: {
        navBar
    },
    setup () {  
        const themeSwitch = ref(true)
        const switchLoading = ref(false)

        const switchBeforeChange = () => {
            switchLoading.value = true
            return new Promise((resolve) => {
                setTimeout(() => {
                switchLoading.value = false
                return resolve(true)
                }, 1000)
            })
            }
        return {
            themeSwitch,
            switchLoading,
            switchBeforeChange
        }
    }
})
</script>

<style scoped>
.section-cover{
    position: absolute;
    height: 100%;
    width: 100%;
    top: 0;
    background: #222831;
    z-index: 1;
    animation: change-theme .5s ease-in-out;
}
.social{
    cursor: pointer;
    overflow: hidden;
    border-radius: 5px 0 0 5px;
    margin-right: 4px;
    padding: 4px 0;
    padding-left: 4px;
    background: rgb(0,173,181);
    background: linear-gradient(90deg, rgba(0,173,181,1) 0%, rgba(238,238,238,1) 100%);
    transition: all .4s ease-in;
}
.social:hover{
    padding-right: 6px;
    padding-left: 6px;
    transition: all .4s ease-in;
}
.social svg{
    color: #393E46;
    height: 18px;
    width: 18px;
}
.email:hover svg{ color: ; }   
.github:hover svg{ color: ; }   
.linkedin:hover svg{ color: ; }  
.facebook:hover svg{ color: ; }  
.instagram:hover svg{ color: ; } 
.twitter:hover svg{ color: ; } 
.social span{
    visibility: hidden;
    max-width: 0;
    color: #222831;
    margin-left: 4px;
    transition: all .5s linear;
    font-size: .8rem;
    //font-weight: bold;
    animation: icons-show-hide .4s linear;
}   
.social:hover span{
    visibility: visible;
    width: auto;
    max-width: 100px;
    transition: all .8s linear;
}
.greetings-title::before{
    content: '';
    position: relative;
    width: 100%;
    border-bottom: 4px solid #222831;
}
.hello-stick-one{
    animation: stick-left-to-right .4s linear;
}
.hello-stick-two{
    animation: stick-right-to-left .4s linear;
}
.fullname{
    animation: slide-left-to-right .5s linear;
}
.img-wrapper{
    perspective: 800px;
}
.img-wrapper::after{
    content: '';
    position: absolute;
    height: 100%;
    width: 100%;
    top: -20px;
    right: -20px    ;
    border-radius: 15px;
    background-color: #00ADB5;  
    transform: rotate3d(0, 1, 0,-30deg);
    z-index: -1 ;
    animation: bg-image-right-to-left .4s ease-in;
}
.ako-img{
    border-radius: 15px;
    object-fit: cover;
    border: 2px solid #00ADB5;
    transform: rotate3d(0, 1, 0,-25deg);
    animation: bg-image-left-to-right  .4s linear;
}
.info-msg{
    animation: hide-show .5s ease-in;
}
.feather-arrow-right{
    animation: arrow-move-right 1.3s linear   infinite;
}
.btn-contact{
    border: 1px solid #00ADB5;
}
.animate-circle-background{
    position: absolute; 
    top: 0;
    left: 0;
    height: 100%;
    width: 100%;
    overflow: hidden;
    z-index: 6  ;
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
@keyframes icons-show-hide {
    0%{
        visibility: visible;
        width: auto;
        max-width: 100px;
    }
    100%{
        visibility: hide;
        max-width: 0;
    }
}
@keyframes stick-right-to-left {
    0%{
        transform: translateX(100%);
    }
    100%{
        transform: translateX(0);
    }
}
@keyframes stick-left-to-right {
    0%{
        transform: translateX(-100%);
    }
    100%{
        transform: translateX(0);
    }
}
@keyframes slide-left-to-right {
    0%{
        transform: translateX(-100%);
    }
    100%{
        transform: translateX(0);
    }
}
@keyframes bg-image-right-to-left {
    0%{
        transform: translateX(-15%);
    }
    100%{
        transform: translateX(0);
        transform: rotate3d(0, 1, 0,-30deg);
    }
}
@keyframes bg-image-left-to-right {
    0%{
        transform: translateX(15%);
    }
    100%{
        transform: translateX(0);
        transform: rotate3d(0, 1, 0,-25deg);
    }
}
@keyframes arrow-move-right {
    0%{
        color: #FFFFFF;
        transform: translate(0);
    }
    50%{
        color: #393E46;
        transform: translate(10px);
    }
    100%{
        color: #393E46;
        transform: translate(0);
    }
}
@keyframes hide-show {
    0%{
        max-height: 0;
    }
    100%{
        opacity: 1;
        max-height: 100px;
    }
}
@keyframes change-theme {
    0%{
        transform: translate(100%, 100%);
        border-radius: 50px;
    }
    
    100%{
        transform: translate(0, 0);
    }
}
</style>