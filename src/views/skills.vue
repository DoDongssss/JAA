<template>
    <section class="flex flex-col items-center justify-center color-EEEEEE skills" id="skills">
        <div class="flex flex-col items-center mb-8">
            <h1 class="font-rowdie font-bold text-[2.5em]">Skills & Experience :</h1>
            <i class="mx-auto">( Experienced Based during OJT - 500hrs )</i>
        </div>
        <div class="flex flex-col items-center mb-4">
            <h5 class="font-bold text-[1.5em]">Front-End Development</h5>
            <!-- <i class="mx-auto">( +500hrs )</i>   -->
        </div>
        <div class="flex flex-wrap gap-4 mt-4">
            <div class="flex flex-col items-center justify-between gap-2 p-4 px-8 bg-c-00ADB5-o rounded-xl skill-item   ">
                <img src="../../src/assets/images/html5.png" alt="" width="90px">
                <span class="font-bold color-EEEEEE tracking-wide text-[.8em]">HTML</span>
            </div>
            <div class="flex flex-col items-center justify-between gap-2 p-4 px-8 bg-c-00ADB5-o rounded-xl skill-item">
                <img src="../../src/assets/images/css.png" alt="" width="90px">
                <span class="font-bold color-EEEEEE tracking-wide text-[.8em]">CSS</span>
            </div>
            <div class="flex flex-col items-center justify-between gap-2 p-4 px-8 bg-c-00ADB5-o rounded-xl skill-item">
                <img src="../../src/assets/images/js.png" alt="" width="90px">
                <span class="font-bold color-EEEEEE tracking-wide text-[.8em]">JS</span>
            </div>
            <div class="flex flex-col items-center justify-between gap-2 p-4 px-8 bg-c-00ADB5-o rounded-xl skill-item">
                <img src="../../src/assets/images/vuejs.png" alt="" width="90px">
                <span class="font-bold color-EEEEEE tracking-wide text-[.8em]">VUEJS</span>
            </div>
            <div class="flex flex-col items-center justify-between gap-2 p-4 px-8 bg-c-00ADB5-o rounded-xl skill-item">
                <img src="../../src/assets/images/wordpress.png" alt="" width="90px">
                <span class="font-bold color-EEEEEE tracking-wide text-[.8em]">WORDPRESS</span>
            </div>
            <div class="flex flex-col items-center justify-between gap-2 p-4 px-8 bg-c-00ADB5-o rounded-xl skill-item">
                <img src="../../src/assets/images/git.png" alt="" width="90px">
                <span class="font-bold color-EEEEEE tracking-wide text-[.8em]">GIT</span>
            </div>
            <div class="flex flex-col items-center justify-between gap-2 p-4 px-8 bg-c-00ADB5-o rounded-xl skill-item">
                <img src="../../src/assets/images/gitlab.png" alt="" width="90px">
                <span class="font-bold color-EEEEEE tracking-wide text-[.8em]">GITLAB</span>
            </div>
        </div>
        <div class="flex flex-col items-center my-8">
            <h1 class="font-rowdie font-bold text-[2.5em]">Secondary :</h1>
            <!-- <i class="mx-auto">( Experienced Based during OJT )</i> -->
        </div>
        <div class="flex flex-col items-center mb-4">
            <h5 class="font-bold text-[1.5em]">Back end Development</h5>
            <!-- <i class="mx-auto">( +500hrs )</i>   -->
        </div>
        <div class="flex gap-4 mt-4">
            <div class="flex flex-col items-center justify-between gap-2 p-4 px-8 bg-c-00ADB5-o rounded-xl skill-item">
                <img src="../../src/assets/images/php.png" alt="" width="90px">
                <span class="font-bold color-EEEEEE tracking-wide text-[.8em]">PHP</span>
            </div>
            <div class="flex flex-col items-center justify-between gap-2 p-4 px-8 bg-c-00ADB5-o rounded-xl skill-item">
                <img src="../../src/assets/images/laravel.png" alt="" width="90px">
                <span class="font-bold color-EEEEEE tracking-wide text-[.8em]">LARAVEL</span>
            </div>
            <div class="flex flex-col items-center justify-between gap-2 p-4 px-8 bg-c-00ADB5-o rounded-xl skill-item">
                <img src="../../src/assets/images/mysql.png" alt="" width="90px">
                <span class="font-bold color-EEEEEE tracking-wide text-[.8em]">MYSQL</span>
            </div>
        </div>
        <div class="flex gap-4 mt-4">
            
        </div>
    </section>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
    setup () {
        

        return {}   
    }
})
</script>

<style scoped>
    .skill-item{
        position: relative; 
        overflow: hidden;
    }
    .skill-item:hover::after{
        content: '';
        position: absolute;
        top: 0;
        border-radius: 0.75rem;
        height: 100%;
        width: 100%;
        background-color: #00ADB5;
        animation: skill-hover-animation .45s ease-in;
        z-index: -1;
    }
    .skill-item img{
        height: 90px!important;
        width: 90px!important;
    }

    @keyframes  skill-hover-animation{
        0%{
            transform: translate(-100%, 100%);
            border-radius: 100%;
        }
        100%{
            transform: translate(0, 0);
        }
    }
</style>