<script setup></script>

<template>
    <h2 class="text-center text-xl font-bold">PROUDLY FEATURED ON:</h2>
    <div class="w-full flex flex-row justify-between mt-3 overflow-x-hidden">
        <div class="flex items-center logo-slide">
            <img src="../assets/img/logo_1.png" alt="">
            <div class="border-r border-slate-300 h-28 ml-2"></div>
        </div>
        <div class="flex items-center logo-slide">
            <img src="../assets/img/logo_02.png" alt="">
            <div class="border-r border-slate-300 h-28 ml-2"></div>
        </div>
        <div class="flex items-center logo-slide">
            <img src="../assets/img/logo_03.png" alt="">
            <div class="border-r border-slate-300 h-28 ml-2"></div>
        </div>
        <div class="flex items-center logo-slide">
            <img src="../assets/img/logo_04.png" alt="">
            <div class="border-r border-slate-300 h-28 ml-2"></div>
        </div>
        <div class="flex items-center logo-slide">
            <img src="../assets/img/logo_05.png" alt="">
            <div class="border-r border-slate-300 h-28 ml-2"></div>
        </div>
        <div class="flex items-center logo-slide">
            <img src="../assets/img/logo_06.png" alt="">
        </div>
    </div>
</template>

<style>
@keyframes slide {
    0% {
        transform: translateX(0);
        /* Start from the initial position */
    }

    100% {
        transform: translateX(-100%);
        /* Keep sliding to the left */
    }
}

.logo-slide {
    animation: slide 10s linear infinite;
    /* Continuously repeat the animation */
    white-space: nowrap;
}</style>
