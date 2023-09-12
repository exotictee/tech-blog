<template>
    <h1 class="text-center font-bold mt-32 text-6xl pb-8">POPULAR POSTS</h1>
    <div class="w-full space-x-3 flex flex-row mt-7 px-32 pb-28">
        <div class="flex flex-col w-1/3 shadow-2xl">
            <NuxtLink to="/">
                <img src="../assets/img/post-01-free-img.jpg" class="w-full" alt="">
            </NuxtLink>
            <div class="px-10 pt-10 pb-5 flex flex-col space-y-3">
                <NuxtLink to="/" class="text-sm font-semibold uppercase tracking-wide text-green-600 ">Cryptocurrency
                </NuxtLink>
                <NuxtLink to="/" class="text-2xl font-extrabold tracking-wide">What are blockchain transaction fees?
                </NuxtLink>
                <p class="pt-5 tracking-wider">
                    Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et.
                </p>
            </div>
        </div>
        <div class="flex flex-col w-1/3 shadow-2xl">
            <NuxtLink to="/">
                <img src="../assets/img/post-01-free-img.jpg" class="w-full" alt="">
            </NuxtLink>
            <div class="px-10 pt-10 pb-5 flex flex-col space-y-3">
                <NuxtLink to="/" class="text-sm font-semibold uppercase tracking-wide text-green-600 ">TECHNOLOGIES
                </NuxtLink>
                <NuxtLink to="/" class="text-2xl font-extrabold tracking-wide">Best Places to Download HTML Templates
                </NuxtLink>
                <p class="pt-5 tracking-wider">
                    Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et.
                </p>
            </div>
        </div>
        <div class="flex flex-col w-1/3 shadow-2xl">
            <NuxtLink to="/">
                <img src="../assets/img/post-01-free-img.jpg" class="w-full" alt="">
            </NuxtLink>
            <div class="px-10 pt-10 pb-5 flex flex-col space-y-3">
                <NuxtLink to="/" class="text-sm font-semibold uppercase tracking-wide text-green-600 ">PROGRAMMING
                </NuxtLink>
                <NuxtLink to="/" class="text-2xl font-extrabold tracking-wide">5 Best Samsung Galaxy Buds Pro Settings
                </NuxtLink>
                <p class="pt-5 tracking-wider">
                    Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et.
                </p>
            </div>
        </div>
    </div>
</template>