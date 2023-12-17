<script>
import { stats } from "./index";
import styles from '../styles'

const { boxWidth, paddingX, flexCenter, flexStart, paddingY, paragraph } = styles;
export default {
    data() {
        console.log(stats);
        return {
            stats,
            boxWidth,
            paddingX,
            flexCenter,
            flexStart,
            paddingY,
            paragraph
        };
    },
};
</script>
  
<template>
    <div>
        <section id="home" :class="['flex md:flex-row flex-col', paddingY]">
            <div :class="['flex-1', flexStart, 'flex-col', 'xl:px-0', 'sm:px-16', 'px-6']">
                <div class="flex flex-row justify-between items-center w-full">
                    <h1
                        class="flex-1 font-poppins font-semibold ss:text-[72px] text-[52px] text-white ss:leading-[100.8px] leading-[75px]">
                        Los Mejores <br class="sm:block hidden" />
                        <span class="text-gradient">Profesionales Calificados</span>
                    </h1>
                </div>
                <p :class="[paragraph, 'max-w-[470px]', 'mt-5']">
                    Conoce algunos de nuestros programas de formacion diseñados y enfocados en tus necesidades!
                </p>


            </div>
            <div :class="['flex-1', 'flex', flexCenter, 'md:my-0', 'my-10', 'relative']">
                <div class="relative flex flex-col-reverse py-16 lg:pt-0 lg:flex-col lg:pb-0">
                    <div
                        class="inset-y-0 top-0 right-0 z-0 w-full max-w-xl px-4 mx-auto md:px-0 lg:pr-0 lg:mb-0 lg:mx-0 lg:w-7/12 lg:max-w-full lg:absolute xl:px-0">
                        <svg class="absolute left-0 hidden h-full text-white transform -translate-x-1/2 lg:block"
                            viewBox="0 0 100 100" fill="currentColor" preserveAspectRatio="none slice">
                            <path d="M50 0H100L50 100H0L50 0Z"></path>
                        </svg>
                        <img class="object-cover w-full h-56 rounded shadow-lg lg:rounded-none lg:shadow-none md:h-96 lg:h-full"
                            src="https://www.microtech.es/hubfs/Fotos%20blog/consultoria_negocios.jpg" alt="" />
                    </div>
                    <div
                        class="relative flex flex-col items-start w-full max-w-xl px-4 mx-auto md:px-0 lg:px-8 lg:max-w-screen-xl">
                        <div class="mb-16 lg:my-40 lg:max-w-lg lg:pr-5">
                            <div class="flex flex-row justify-between items-center w-full">
                                <h1
                                    class="flex-1 font-poppins font-semibold ss:text-[72px] text-[52px] text-slate-600 ss:leading-[100.8px] leading-[75px]">
                                    Calidad <br class="sm:block hidden" />
                                    <span class="text-gradient">Atención y Responsabilidad</span>
                                </h1>
                            </div>
                        </div>
                    </div>
                </div>
                <div class="b h-16 w-64 flex justify-center items-center absolute z-[10] top-6 right-0">
                    <div
                        class="i h-16 w-64 bg-blue-300 items-center rounded-xl shadow-2xl cursor-pointer absolute overflow-hidden transform hover:scale-x-110 hover:scale-y-105 transition duration-300 ease-out">
                    </div>
                    <a href="#footer" class="text-center text-white font-semibold z-10 pointer-events-none">Contáctanos</a>
                    <span class="absolute flex h-6 w-6 top-0 right-0 transform translate-x-2.5 -translate-y-2.5">
                        <span
                            class="animate-ping absolute inline-flex h-full w-full rounded-full bg-purple-400 opacity-75"></span>
                        <span class="absolute inline-flex rounded-full h-6 w-6 bg-purple-500"></span>
                    </span>
                </div>
            </div>
            <div class="flex items-end justify-end fixed bottom-0 right-0 mb-4 mr-4 z-10">
                <div>
                    <a title="Whatsapp"
                        href="https://api.whatsapp.com/send/?phone=%2B5491159554409&text&type=phone_number&app_absent=0"
                        target="_blank"
                        class="block w-16 h-16 rounded-full transition-all shadow hover:shadow-lg transform hover:scale-110 hover:rotate-12">
                        <img class="object-cover object-center w-full h-full rounded-full"
                            src="https://2.bp.blogspot.com/-QfS1hyElLFk/XDdD551JV7I/AAAAAAAAGu0/ZwfoMBwMoiUAzSCHhP4QvHn_KyjaeecWQCK4BGAYYCw/s1600/logo%2Bwhatsapp.png" />
                    </a>
                </div>
            </div>
        </section>
        <section :class="[flexCenter, 'flex-row', 'flex-wrap', 'sm:mb-20', 'mb-6']">
            <div v-for="stat in stats" :key="stat.id" class="flex-1 flex justify-start items-center flex-row m-3">
                <p class="font-poppins font-normal xs:text-[20.45px] text-[15.45px] xs:leading-[26.58px] 
                    leading-[21.58px] text-gradient uppercase ml-3">
                    {{ stat.title }}
                </p>
            </div>
        </section>
    </div>
</template>

  