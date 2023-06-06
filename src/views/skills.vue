<template>
    <section class="h-auto lg:h-auto abs-center flex-col py-[5rem]" id="skills">
        <div class="flex flex-col items-center mb-8" data-aos="zoom-in">
            <h1 class="font-rowdie font-bold text-[2em] section-title">Skills & Experience</h1>
            <i class="mx-auto">( Experienced Based during OJT - 500hrs )</i>
        </div>
        <div class="flex flex-col items-center mb-4" data-aos="zoom-in-down">
            <h5 class="font-bold text-[1.3em]">Front end Development</h5>
            <!-- <i class="mx-auto">( +500hrs )</i>   -->
        </div>
        <div class="flex flex-wrap justify-center gap-4 mt-4" data-aos="fade-right">
            <div class="flex flex-col items-center justify-between gap-2 p-4 px-8 bg-c-00ADB5-trans rounded-xl skill-item   ">
                <img src="../../images/html.png" alt="" width="90px">
                <span class="font-bold color-EEEEEE tracking-wide text-[.8em]">HTML</span>
            </div>
            <div class="flex flex-col items-center justify-between gap-2 p-4 px-8 bg-c-00ADB5-trans rounded-xl skill-item">
                <img src="../../images/css.png" alt="" width="90px">
                <span class="font-bold color-EEEEEE tracking-wide text-[.8em]">CSS</span>
            </div>
            <div class="flex flex-col items-center justify-between gap-2 p-4 px-8 bg-c-00ADB5-trans rounded-xl skill-item">
                <img src="../../images/js.png" alt="" width="90px">
                <span class="font-bold color-EEEEEE tracking-wide text-[.8em]">JS</span>
            </div>
            <div class="flex flex-col items-center justify-between gap-2 p-4 px-8 bg-c-00ADB5-trans rounded-xl skill-item">
                <img src="../../images/vuejs.png" alt="" width="90px">
                <span class="font-bold color-EEEEEE tracking-wide text-[.8em]">VUEJS</span>
            </div>
            <div class="flex flex-col items-center justify-between gap-2 p-4 px-8 bg-c-00ADB5-trans rounded-xl skill-item">
                <img src="../../images/wordpress.png" alt="" width="90px">
                <span class="font-bold color-EEEEEE tracking-wide text-[.8em]">WORDPRESS</span>
            </div>
            <div class="flex flex-col items-center justify-between gap-2 p-4 px-8 bg-c-00ADB5-trans rounded-xl skill-item">
                <img src="../../images/git.png" alt="" width="90px">
                <span class="font-bold color-EEEEEE tracking-wide text-[.8em]">GIT</span>
            </div>
            <!-- <div class="flex flex-col items-center justify-between gap-2 p-4 px-8 bg-c-00ADB5-trans rounded-xl skill-item">
                <img src="../../images/gitlab.png" alt="" width="90px">
                <span class="font-bold color-EEEEEE tracking-wide text-[.8em]">GITLAB</span>
            </div> -->
        </div>
        <div class="flex flex-col items-center my-8" data-aos="zoom-in">
            <h1 class="font-rowdie font-bold text-[2em]">Secondary</h1>
            <!-- <i class="mx-auto">( Experienced Based during OJT )</i> -->
        </div>
        <div class="flex flex-col items-center mb-4" data-aos="zoom-in-down">
            <h5 class="font-bold text-[1.3em]">Back end Development</h5>
            <!-- <i class="mx-auto">( +500hrs )</i>   -->
        </div>
        <div class="flex flex-wrap justify-center gap-4 mt-4" data-aos="fade-left">
            <div class="flex flex-col items-center justify-between gap-2 p-4 px-8 bg-c-00ADB5-trans rounded-xl skill-item">
                <img src="../../images/php.png" alt="" width="90px">
                <span class="font-bold color-EEEEEE tracking-wide text-[.8em]">PHP</span>
            </div>
            <div class="flex flex-col items-center justify-between gap-2 p-4 px-8 bg-c-00ADB5-trans rounded-xl skill-item">
                <img src="../../images/laravel.png" alt="" width="90px">
                <span class="font-bold color-EEEEEE tracking-wide text-[.8em]">LARAVEL</span>
            </div>
            <div class="flex flex-col items-center justify-between gap-2 p-4 px-8 bg-c-00ADB5-trans rounded-xl skill-item">
                <img src="../../images/mysql.png" alt="" width="90px">
                <span class="font-bold color-EEEEEE tracking-wide text-[.8em]">MYSQL</span>
            </div>
            <div class="flex flex-col items-center justify-between gap-2 p-4 px-8 bg-c-00ADB5-trans rounded-xl skill-item">
                <img src="../../images/java.png" alt="" width="90px">
                <span class="font-bold color-EEEEEE tracking-wide text-[.8em]">JAVA</span>
            </div>
            <div class="flex flex-col items-center justify-between gap-2 p-4 px-8 bg-c-00ADB5-trans rounded-xl skill-item">
                <img src="../../images/c++.png" alt="" width="90px">
                <span class="font-bold color-EEEEEE tracking-wide text-[.8em]">C++</span>
            </div>
            <div class="flex flex-col items-center justify-between gap-2 p-4 px-8 bg-c-00ADB5-trans rounded-xl skill-item">
                <img src="../../images/flutter.png" alt="" width="90px">
                <span class="font-bold color-EEEEEE tracking-wide text-[.8em]">FLUTTER</span>
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
.skill-item img{
    height: 90px!important;
    width: 90px!important;
}
.skill-item:hover img{
    filter: drop-shadow(0 0 5px #eee);
    transition: all .4s ease-in;
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