<template>
    <nav class="w-full flex py-6 justify-between items-center navbar">
        <img :src="kairos" class="w-[134px] h-[32px]" />

        <ul class="list-none sm:flex hidden justify-end items-center flex-1">
            <li v-for="(nav, index) in navLinks" :key="nav.id" :class="['font-poppins', 'font-normal', 'cursor-pointer', 'text-[16px]',
                active === nav.title ? 'text-white' : 'text-slate-400',
                index === navLinks.length - 1 ? 'mr-0' : 'mr-10']" @click="setActive(nav.title)">
                <a :href="nav.href">{{ nav.title }}</a>
            </li>
        </ul>

        <div class="sm:hidden flex flex-1 justify-end items-center">
            <img :src="toggle ? close : menu" alt="menu" class="w-[28px] h-[28px] object-contain"
                @click="setToggle(!toggle)" />

            <div :class="['p-6', 'bg-black-gradient', 'absolute', 'top-20', 'right-0', 'mx-4', 'my-2', 'min-w-[140px]', 'rounded-xl', 'sidebar',
                toggle ? '' : 'hidden']">
                <ul class="list-none flex justify-end items-start flex-1 flex-col">
                    <li v-for="(nav, index) in navLinks" :key="nav.id" :class="['font-poppins', 'font-normal', 'cursor-pointer', 'text-[16px]',
                        active === nav.title ? 'text-white' : 'text-slate-400',
                        index === navLinks.length - 1 ? 'mr-0' : 'mr-10']" @click="setActive(nav.title)">
                        <a :href="nav.href">{{ nav.title }}</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</template>
  
<script setup>
import { ref } from "vue";
import kairos from "../assets/kairos.png";
import menu from "../assets//menu.png";
import close from "../assets//close.png";
import { navLinks } from "../constants/index";

const active = ref("Home");
const toggle = ref(false);

const setActive = (title) => {
    active.value = title;
};

const setToggle = () => {
    toggle.value = !toggle.value;
};
</script>
  
<style scoped></style>
  