<template>
    <nav class="hidden lg:flex gap-6 z-20">
        <li class="list-none overflow-hidden nav-item" @click="checkRoute('main')" :class="[routeName === 'main' ? 'active' : '']">
            <a href="#main" class="flex">
                <span class="relative hidden lg:block text-black tracking-wider text-[1.05rem]">Home</span>
            </a>
        </li>
        
        <li class="list-none overflow-hidden nav-item" @click="checkRoute('about')" :class="[routeName === 'about' ? 'active' : '']">
            <a href="#about" class="flex">
                <span class="relative hidden lg:block text-black tracking-wider text-[1.05rem]">About</span>
            </a>
        </li>

        <li class="list-none overflow-hidden nav-item" @click="checkRoute('skills')" :class="[routeName === 'skills' ? 'active' : '']">
            <a href="#skills" class="flex">
                <span class="relative hidden lg:block text-black tracking-wider text-[1.05rem]">Skills</span>
            </a>
        </li>

        <li class="list-none overflow-hidden nav-item" @click="checkRoute('project')" :class="[routeName === 'project' ? 'active' : '']">
            <a href="#project" class="flex">    
                <span class="relative hidden lg:block text-black tracking-wider text-[1.05rem]">Project</span>
            </a>
        </li>

        <li class="list-none overflow-hidden nav-item" @click="checkRoute('contact')" :class="[routeName === 'contact' ? 'active' : '']">
            <a href="#contact" class="flex">
                <span class="relative hidden lg:block text-black tracking-wider text-[1.05rem]">Contact</span>
            </a>
        </li>
    </nav>

    <!-- dropdown navigation -->
    <nav class="fixed flex lg:hidden py-2 px-6 top-[calc(100vh-50px)] z-[99999] bg-c-00ADB5-trans-med rounded-xl">
        <li class="dd-nav-item active">
            <svg xmlns="http://www.w3.org/2000/svg" width="25" height="25" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1" stroke-linecap="round" stroke-linejoin="round" class="feather feather-home">
                <path d="M3 9l9-7 9 7v11a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z"></path>
                <polyline points="9 22 9 12 15 12 15 22"></polyline>
            </svg>
        </li>
        <li class="dd-nav-item">
            <svg xmlns="http://www.w3.org/2000/svg" width="25" height="25" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1" stroke-linecap="round" stroke-linejoin="round" class="feather feather-user">
                <path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"></path> 
                <circle cx="12" cy="7" r="4"></circle>  
            </svg>
        </li>
        <li class="dd-nav-item">
            <svg xmlns="http://www.w3.org/2000/svg" width="25" height="25" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1" stroke-linecap="round" stroke-linejoin="round" class="feather feather-tool">
                <path d="M14.7 6.3a1 1 0 0 0 0 1.4l1.6 1.6a1 1 0 0 0 1.4 0l3.77-3.77a6 6 0 0 1-7.94 7.94l-6.91 6.91a2.12 2.12 0 0 1-3-3l6.91-6.91a6 6 0 0 1 7.94-7.94l-3.76 3.76z"></path>
            </svg>
        </li>
        <li class="dd-nav-item">
            <svg xmlns="http://www.w3.org/2000/svg" width="25" height="25" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1" stroke-linecap="round" stroke-linejoin="round" class="feather feather-briefcase">
                <rect x="2" y="7" width="20" height="14" rx="2" ry="2"></rect>
                <path d="M16 21V5a2 2 0 0 0-2-2h-4a2 2 0 0 0-2 2v16"></path>
            </svg>
        </li>
        <li class="dd-nav-item">
            <svg xmlns="http://www.w3.org/2000/svg" width="25" height="25" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1" stroke-linecap="round" stroke-linejoin="round" class="feather feather-phone">
                <path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"></path>
            </svg>
        </li>
    </nav>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue'
import { useRouter, useRoute } from 'vue-router'

export default defineComponent({
    setup () {
        const location = useRoute();

        return {
            location,
        }
    },
    data(){
        return {
            routeName : 'main'
        }
    },
    methods: {
        checkRoute(newRoute : string){
            this.routeName = newRoute
            console.log(this.routeName)
        }
    }
})
</script>

<style>
    .nav-item{
        overflow: hidden;
        cursor: pointer;
    }
    .nav-item svg{
        color: var(--secondary);
        margin-right: 5px;
    }
    .nav-item:hover svg{
        fill: var(--secondary);
        animation: bounce 1s infinite;
    }
    .nav-item.active svg{
        color: var(--tertiary);
        fill: none;
        animation: bounce 1s infinite;
    }
    .nav-item.active span{
        color: var(--tertiary);
    }
    .nav-item:hover span::after,
    .nav-item.active span::after{
        content: '';
        position: absolute;
        height: 100%;
        width: 100%;
        inset: 0;
        border-bottom: 2px solid var(--secondary);
        animation: left-to-right .2s linear;
    }
    .nav-item.active span::after{
        border-bottom: 2px solid var(--tertiary);
    }

    .dd-nav-item{
        list-style-type: none;
        animation: bot-to-top .6s linear;
        cursor: pointer;
    }
    .dd-nav-item svg{
        color: var(--primary);
        fill: var(--quaternary);
        margin-right: 15px;
    }
    .dd-nav-item.active svg{
        fill: var(--tertiary);
        animation: bounce 1s infinite;
    }
</style>