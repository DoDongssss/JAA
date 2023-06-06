<template>
    <section class="relative h-auto lg:h-[calc(100vh-3rem)] bg-c-EEEEEE rounded-2xl index p-[1rem] color-393E46">
        <div class="h-[50px] flex flex-row justify-between bg-transparent z-20">
            <span class="font-montserrat font-bold text-[1.5rem] tracking-wider">
                <span class="color-00ADB5 font-bold">D</span>o<span class="color-00ADB5 font-bold">D</span>ong
            </span> 
            <div class="w-fit flex items-center">
                <navigation/>
            </div>
            <div class="hidden md:flex abs-center color-393E46 rounded-b-xl px-2 z-20">
                <div>
                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-moon cursor-pointer" :class="[ mode ? 'block' : 'hidden']" 
                    @click="switchmode">
                        <path d="M21 12.79A9 9 0 1 1 11.21 3 7 7 0 0 0 21 12.79z"></path>
                    </svg>

                    <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="feather feather-sun cursor-pointer" :class="[mode ? 'hidden' : 'block']" 
                    @click="switchmode">
                        <circle cx="12" cy="12" r="5"></circle>
                        <line x1="12" y1="1" x2="12" y2="3"></line><line x1="12" y1="21" x2="12" y2="23"></line>
                        <line x1="4.22" y1="4.22" x2="5.64" y2="5.64"></line><line x1="18.36" y1="18.36" x2="19.78" y2="19.78"></line>
                        <line x1="1" y1="12" x2="3" y2="12"></line>
                        <line x1="21" y1="12" x2="23" y2="12"></line>
                        <line x1="4.22" y1="19.78" x2="5.64" y2="18.36"></line>
                        <line x1="18.36" y1="5.64" x2="19.78" y2="4.22"></line>
                    </svg>
                </div>
            </div>  
        </div>
        <main class="h-auto lg:h-[calc(100%-50px)] w-full flex flex-col lg:flex-row bg-transparent z-20">
            <div class="abs-center flex-col h-full w-full lg:w-[50%] color-393E46 p-[1rem]">
                <div class="w-[80%] flex items-center justify-between overflow-hidden">
                    <span class="w-[35%] border-b-[2px] border-[#00ADB5] hello-stick-left"></span>
                        <span class="tracking-[5px] text-sm color-393E46 px-2 dev-greet">HELLO I'M</span>
                    <span class="w-[35%] border-b-[2px] border-[#00ADB5] hello-stick-right"></span>
                </div>  
                <h1 class="abs-center w-[80%] font-[900] text-[2.5rem]  lg:text-[3rem] 2xl:text-[3rem] font-montserrat   tracking-wider overflow-hidden dev-name">Johnny A. Asumbra</h1>
                <p class="w-[80%] text-base text-center lg:text-justify mt-4 info-msg overflow-hidden dev-info">
                    Welcome to my portfolio! I'm a web developer passionate about developing websites. Explore my work, testimonials, and professional background. Let's connect and collaborate on exciting projects. Thank you for visiting!
                </p>
                <socials class="w-[80%]"/>
                <div class="w-[80%] flex items-center justify-center lg:items-start lg:justify-start mt-7 z-20"> 
                    <button type="button" class="mr-3 py-[10.5px] px-5 bg-c-00ADB5 rounded-[5px] tracking-wide text-white">Download CV</button>
                    <button type="button" class="flex py-[10.5px] px-5 rounded-[5px] tracking-wide text-[#393E46] border border-[#00ADB5] ">
                        Contact Me
                        <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1" stroke-linecap="round" stroke-linejoin="round" class="feather feather-arrow-right ml-1">
                            <line x1="5" y1="12" x2="19" y2="12"></line>
                            <polyline points="12 5 19 12 12 19"></polyline>
                        </svg>
                    </button>
                </div>
            </div>
            <div class="abs-center h-full w-full lg:w-[50%] mt-10 lg:mt-0">
                <div class="h-[300px] w-[300px] md:h-[400px] md:w-[400px] img-wrapper z-20">
                    <img src="../../public/images/ako.jpg" alt="" class="h-full w-full">
                </div>
            </div>
        </main>
        <bgBoxAnimation/>
    </section>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue'
import navigation from '../../src/components/nav.vue'
import bgBoxAnimation from '../../src/components/bg-box.vue'
import socials from '../../src/components/social.vue'

export default defineComponent({
    components: {
        navigation,
        bgBoxAnimation,
        socials
    },
    setup () {

        return {
            
        }
    },
    data(){
        return{
            mode: false
        }
    },
    methods: {
        switchmode(): boolean{
           return this.mode = !this.mode
        }
    }
})
</script>

<style>
.hello-stick-left{
    animation: left-to-right .6s ease-in;
}
.dev-greet{
    animation: opacity .6s ease-in;
}
.hello-stick-right{
    animation: right-to-left .6s ease-in;
}
.dev-name{
    animation: left-to-right .6s ease-in;
}
.dev-info{
    animation: max-height .6s linear;
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
    right: -20px;
    border-radius: 15px;
    background-color: #00ADB5;  
    transform: rotate3d(0, 1, 0,-30deg);
    z-index: -1 ;
    animation: image-right-to-left .6s linear;
}
.img-wrapper img{
    border-radius: 15px;
    object-fit: cover;
    border: 2px solid #00ADB5;
    transform: rotate3d(0, 1, 0,-25deg);
    animation: image-left-to-right  .7s linear;
}

</style> 