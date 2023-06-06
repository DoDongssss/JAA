<template>
    <section class="h-auto abs-center flex-col py-[5rem]" id="about">
        <h1 class="font-rowdie font-bold text-[2em] mb-5 py-1 section-title"  data-aos="zoom-in">Educational Background</h1>
        <div class="flex flex-wrap gap-2">
            <div class="flex h-[400px] min-w-[300px] w-[calc(100%/4-.5rem)] rounded-xl bg-c-00ADB5-trans-med py-10 px-5" data-aos="fade-right">
                <div class="abs-center mr-2 label-stick">
                    <span></span>
                </div>
                <div class="flex flex-col">
                    <h5 class="font-bold text-[1em]">Notre Dame of Marbel University</h5>
                    <span class="text-[.6em]">( NDMU Complex, NDMU Basketball Court (outdoor), Rafael Alunan Ave, Poblacion, Koronadal City, 9506 South Cotabato )</span>
                    <span class="bg-c-393E46 w-fit px-2 mt-2 rounded skew-y-2">2019 - 2023</span>
                    <img src="../../public/images/college.jpg" alt="" class="px-2 py-4 object-cover rounded-[30px] educ-img">
                </div>
            </div>
            <div class="flex h-[400px] min-w-[300px] w-[calc(100%/4-.5rem)] rounded-xl bg-c-00ADB5-trans-med py-10 px-5" data-aos="fade-up-right">
                <div class="abs-center mr-2 label-stick">
                    <span></span>
                </div>
                <div class="flex flex-col">
                    <h5 class="font-bold text-[1em]">STI College Koronadal</h5>
                    <span class="text-[.6em]">( Brgy Santa Lucia St, Poblacion, Koronadal City, 9506 South Cotabato )</span>
                    <span class="bg-c-393E46 w-fit px-2 mt-2 rounded skew-y-2">2017 - 2019</span>
                    <img src="../../public/images/shs.jpg" alt="" class="px-2 py-4 object-cover rounded-[30px] educ-img">
                </div>
            </div>
            <div class="flex h-[400px] min-w-[300px] w-[calc(100%/4-.5rem)] rounded-xl bg-c-00ADB5-trans-med py-10 px-5" data-aos="fade-up-left">
                <div class="abs-center mr-2 label-stick">
                    <span></span>
                </div>
                <div class="flex flex-col">
                    <h5 class="font-bold text-[1em]">Tampakan National High School</h5>
                    <span class="text-[.6em]">( CWXG+36R, Poblacion, Tampakan, 9507 South Cotabato )</span>
                    <span class="bg-c-393E46 w-fit px-2 mt-2 rounded skew-y-2">2013 - 2017</span>
                    <img src="../../public/images/hs.jpg" alt="" class="px-2 py-4 object-cover rounded-[30px] mt-[10px] educ-img">
                </div>
            </div>
            <div class="flex h-[400px] min-w-[300px] w-[calc(100%/4-.5rem)] rounded-xl bg-c-00ADB5-trans-med py-10 px-5" data-aos="fade-left">
                <div class="abs-center mr-2 label-stick">
                    <span></span>
                </div>
                <div class="flex flex-col">
                    <h5 class="font-bold text-[1em]">Lanton Elementary School</h5>
                    <span class="text-[.6em]">( PUROK-5 LANTON, E Salamanca Ave, General Santos City, 9500 South Cotabato )</span>
                    <span class="bg-c-393E46 w-fit px-2 mt-2 rounded skew-y-2">2007 - 2013</span>
                    <img src="../../public/images/noimage.png" alt="" class="px-2 py-4 object-cover rounded-[30px] educ-img">
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
    .label-stick{
        height: 100%;
        width: 50px;
    }
    .label-stick span{
        position: relative;
        height: 100%;
        width: 1px;
        background-color: var(--secondary);
        border-radius: 30px;
        display: flex;
        justify-content: center;
    }
    .label-stick span::after{
        content: '';
        position: absolute;
        top: 0;
        height: 12px;
        width: 12px;
        border-radius: 100%;
        background-color: var(--tertiary);
    }
    .label-stick span::before{
        content: '';
        position: absolute;
        bottom: 0;
        height: 12px;
        width: 12px;
        border-radius: 100%;
        background-color: var(--tertiary);
    }
    .educ-img{
        filter: grayscale();
        transform: skew(-5deg);
        transition: all .3s linear;
    }
    .educ-img:hover{
        filter: none;
        transform: skew(0);
        transition: all .3s linear;
    }
</style>