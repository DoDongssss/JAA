<template>
    <div class="h-[50px] w-[100vw] flex items-center justify-between bg-c-00ADB5-trans ml-[-29px] px-[29px]">
        <div>
            <div class="flex flex-wrap gap-3 ">
                <a href="https://github.com/DoDongssss" target="_blank" class="social-item">
                    <svg xmlns="http://www.w3.org/2000/svg" width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1" stroke-linecap="round" stroke-linejoin="round" class="feather feather-github"><path d="M9 19c-5 1.5-5-2.5-7-3m14 6v-3.87a3.37 3.37 0 0 0-.94-2.61c3.14-.35 6.44-1.54 6.44-7A5.44 5.44 0 0 0 20 4.77 5.07 5.07 0 0 0 19.91 1S18.73.65 16 2.48a13.38 13.38 0 0 0-7 0C6.27.65 5.09 1 5.09 1A5.07 5.07 0 0 0 5 4.77a5.44 5.44 0 0 0-1.5 3.78c0 5.42 3.3 6.61 6.44 7A3.37 3.37 0 0 0 9 18.13V22"></path></svg> 
                    <span>Github</span>
                </a>
                <a href="https://www.linkedin.com/in/johnny-asumbra-0b8b5a25a/" target="_blank" class="social-item">
                    <svg xmlns="http://www.w3.org/2000/svg" width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1" stroke-linecap="round" stroke-linejoin="round" class="feather feather-linkedin">
                        <path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"></path><rect x="2" y="9" width="4" height="12"></rect><circle cx="4" cy="4" r="2"></circle></svg>
                    <span>LinkedIn</span>
                </a>
                <a href="https://www.instagram.com/asumbra_/" target="_blank" class="social-item">
                    <svg xmlns="http://www.w3.org/2000/svg" width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1" stroke-linecap="round" stroke-linejoin="round" class="feather feather-instagram">
                        <rect x="2" y="2" width="20" height="20" rx="5" ry="5"></rect><path d="M16 11.37A4 4 0 1 1 12.63 8 4 4 0 0 1 16 11.37z"></path><line x1="17.5" y1="6.5" x2="17.51" y2="6.5"></line></svg>
                    <span>Instagram</span>
                </a>
                <a href="https://www.facebook.com/TuDesse/" target="_blank" class="social-item">
                    <svg xmlns="http://www.w3.org/2000/svg" width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1" stroke-linecap="round" stroke-linejoin="round" class="feather feather-facebook"><path d="M18 2h-3a5 5 0 0 0-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 0 1 1-1h3z"></path></svg>
                    <span>Facebook</span>
                </a>
                <a href="https://twitter.com/xchitts" target="_blank" class="social-item">
                    <svg xmlns="http://www.w3.org/2000/svg" width="15" height="15" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1" stroke-linecap="round" stroke-linejoin="round" class="feather feather-twitter"><path d="M23 3a10.9 10.9 0 0 1-3.14 1.53 4.48 4.48 0 0 0-7.86 3v1A10.66 10.66 0 0 1 3 4s-4 9 5 13a11.64 11.64 0 0 1-7 2c9 5 20 0 20-11.5a4.5 4.5 0 0 0-.08-.83A7.72 7.72 0 0 0 23 3z"></path></svg>
                    <span>Twitter</span>
                </a>
            </div>
        </div>
        <div>
            <p>Thank you for visiting my page!</p>
        </div>
        <div>
            <span class="">© 2023 Asumbra</span>
        </div>
    </div>
</template>

<script lang="ts">
import { defineComponent } from 'vue'
import socials from '../../src/components/social.vue'

export default defineComponent({
    components: {
        socials
    },
    setup () {
        

        return {}
    }
})
</script>

<style scoped>
.social-item{
    position: relative;
    display: flex;
    align-items: center;
    justify-content: center;
    padding: 3px;
    padding: 3px 6px;
    border: 1px solid #00ADB5;
    border-radius: 50%;
    background-color: rgba(0, 173, 181, .5);
    z-index: 20;
    gap: 0;
    transition: all .5s linear;
}
.social-item span{
    width: 0;
    max-width: 0;
    overflow: hidden;
    transition: all .5s linear;
    font-size: .8rem;
}
.social-item:hover span{
    width: 60px;
    max-width: 150px;
    display: flex;
    transition: all .5s linear;
}
.social-item:hover{
    gap: 5px;
    background-color: rgb(0, 173, 181);
    border-color: rgba(0, 173, 181, .5);
    border-radius: 5px;
    transition: all .3s ease-in;
    animation: bounce 1s linear infinite;
} 
</style>