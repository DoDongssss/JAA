<template>
    <section class="h-auto abs-center flex-col py-[5rem]" id="project">
        <h1 class="font-rowdie font-bold text-[2em] mb-5 section-title" data-aos="zoom-in">Projects</h1>
        <div class="abs-center mt-4 flex-col">
            <div class="h-[350px] w-[1000px] flex gap-3 bg-c-393E46 rounded-xl p-4 translate-x-[-100px] border-l-[2.5px] border-[#00ADB5] first-proj" data-aos="zoom-in-right">
                <div class="h-full w-[65%]">
                    <img src="../../public/images/project2.jpg" alt="" class="rounded-xl object-fill h-full w-full">
                </div>
                <div class="h-full w-[35%] flex flex-col color-EEEEEE font-montserrat">
                    <h2 class="text-[2em] font-[900] color-00ADB5">Web Portfolio</h2>
                    <p class="text-[.9rem] mt-2">This is my personal portfolio, it contains my information about skills, experience and projects.</p>
                    <div class="mt-4 flex flex-wrap gap-2">
                        <span class="px-2 py-1 rounded-xl bg-c-222831 font-bold text-[.7rem]">Vue</span>
                        <span class="px-2 py-1 rounded-xl bg-c-222831 font-bold text-[.7rem]">HTML</span>
                        <span class="px-2 py-1 rounded-xl bg-c-222831 font-bold text-[.7rem]">TailWindCSS</span>
                        <span class="px-2 py-1 rounded-xl bg-c-222831 font-bold text-[.7rem]">JS</span>
                        <span class="px-2 py-1 rounded-xl bg-c-222831 font-bold text-[.7rem]">ElementPlus</span>
                    </div>
                    <div class="mt-6">
                        <button class="mr-3 py-2 px-4 bg-c-00ADB5 rounded-md tracking-wide"> take a look </button>
                    </div>
                </div>
            </div>
            <div class="h-[350px] w-[1000px] flex gap-3 bg-c-393E46 rounded-xl p-4 mt-5 translate-x-[100px] border-r-[2.5px] border-[#00ADB5] second-proj" data-aos="zoom-out">
                <div class="h-full w-[65%] order-2">
                    <img src="../../public/images/project1.jpg" alt="" class="rounded-xl object-fill h-full w-full">
                </div>
                <div class="h-full w-[35%] flex flex-col color-EEEEEE font-montserrat order-1">
                    <h2 class="text-[2em] font-[900] color-00ADB5">DocKoTo</h2>
                    <p class="text-[.9rem] mt-2">DocKoTo is a mobile app. It offers a free, easy, and secure way to connect with medical specialists for online consultation anytime, anywhere.</p>
                    <div class="mt-4">
                        <span class="px-2 py-1 rounded-xl bg-c-222831 font-bold text-[.7rem]">wordpress</span>
                    </div>
                    <div class="mt-5">
                        <button class="mr-3 py-2 px-4 bg-c-222831 rounded-md tracking-wide bg-c-00ADB5"> take a look </button>
                    </div>
                </div>
            </div>
            <div class="h-[350px] w-[1000px] flex gap-3 bg-c-393E46 rounded-xl p-4 mt-5 translate-x-[-100px] border-l-2 border-[#00ADB5] third-proj" data-aos="zoom-in-right">
                <div class="h-full w-[65%]">
                    <img src="../../public/images/project3.jpg" alt="" class="rounded-xl object-fill h-full w-full">
                </div>
                <div class="h-full w-[35%] flex flex-col color-EEEEEE font-montserrat">
                    <h2 class="text-[2em] font-[900] color-00ADB5">VME SaaS</h2>
                    <p class="text-[.9rem] mt-2">VME SaaS is a virtual Media Event which can manage an event, this project is still on going.</p>
                    <div class="flex flex-wrap gap-2 mt-4">
                        <span class="px-2 py-1 rounded-xl bg-c-222831 font-bold text-[.7rem]">HTML</span>
                        <span class="px-2 py-1 rounded-xl bg-c-222831 font-bold text-[.7rem]">Bootstrap</span>
                        <span class="px-2 py-1 rounded-xl bg-c-222831 font-bold text-[.7rem]">JS</span>
                        <span class="px-2 py-1 rounded-xl bg-c-222831 font-bold text-[.7rem]">Vue</span>
                        <span class="px-2 py-1 rounded-xl bg-c-222831 font-bold text-[.7rem]">ElementPlus</span>
                        <span class="px-2 py-1 rounded-xl bg-c-222831 font-bold text-[.7rem]">Ant-Design</span>
                    </div>
                    <div class="mt-5">
                        <button class="mr-3 py-2 px-4 bg-c-222831 rounded-md tracking-wide bg-c-00ADB5"> take a look </button>
                    </div>
                </div>
            </div>
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
.first-proj,
.third-proj{
    background: rgb(0,173,181);
background: linear-gradient(90deg, rgba(0,173,181,0.5) 0%, rgba(57,62,70,1) 100%);
transform: translateX(-100px) !important;
}
.second-proj{
    background: rgb(57,62,70);
background: linear-gradient(90deg, rgba(57,62,70,1) 0%, rgba(0,173,181,0.5) 100%);
transform: translateX(100px) !important;
}
</style>