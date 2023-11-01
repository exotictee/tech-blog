<template>
    <div :class="[$route.path === '/' ? 'bg-gray-200' : 'bg-white', 'pb-24']">
        <!-- Show h1 tag only on the index page -->
        <h1 v-if="$route.path === '/'" class="text-5xl font-extrabold pt-32 pb-20 text-center">DEALS</h1>

        <!-- Display a vertical lime line on other pages -->
        <div v-else>
            <VertLine />
        </div>

        <div class="flex flex-row w-full px-32 space-x-3 pt-24">
            <div class="w-1/3 flex flex-col">
                <NuxtLink to="/">
                    <img src="../assets/img/purple-logoipsum.jpg" class="w-full shadow-2xl" alt="">
                </NuxtLink>
                <div class="flex flex-col mt-8 text-center px-10 space-y-2">
                    <NuxtLink to="/" class="text-green-600 font-semibold text-lg">SAVE 66%</NuxtLink>
                    <NuxtLink to="/" class="font-extrabold text-3xl -tracking-wider">LogoIpsum Hosting Coupon: Save 66% +
                        Free Domain</NuxtLink>
                </div>
                <div v-if="$route.path !== '/'">
                    <div class="w-full flex items-center justify-center mt-10">
                        <button class="text-white px-10 py-4 tracking-wider rounded-md bg-lime-600 hover:bg-lime-500">GET
                            NOW</button>
                    </div>
                    <div class="flex items-center mt-5 justify-center">
                        <button class="text-slate-500 tracking-wide">READ MORE</button>
                    </div>
                </div>

            </div>
            <div class="w-1/3 flex flex-col">
                <NuxtLink to="/">
                    <img src="../assets/img/l_blue-logoipsum.jpg" class="w-full shadow-2xl" alt="">
                </NuxtLink>
                <div class="flex flex-col mt-8 text-center px-10 space-y-2">
                    <NuxtLink to="/" class="text-green-600 font-semibold text-lg">UP TO 63%</NuxtLink>
                    <NuxtLink to="/" class="font-extrabold text-3xl -tracking-wider">LogoIpsum Hosting Coupon: Save 66% +
                        Free Domain</NuxtLink>
                </div>
                <div v-if="$route.path !== '/'">
                    <div class="w-full flex items-center justify-center mt-10">
                        <button class="text-white px-10 py-4 tracking-wider rounded-md bg-lime-600 hover:bg-lime-500">GET
                            NOW</button>
                    </div>
                    <div class="flex items-center mt-5 justify-center">
                        <button class="text-slate-500 tracking-wide">READ MORE</button>
                    </div>
                </div>
            </div>
            <div class="w-1/3 flex flex-col">
                <NuxtLink to="/">
                    <img src="../assets/img/lemon-logoipsum.jpg" class="w-full shadow-2xl" alt="">
                </NuxtLink>
                <div class="flex flex-col mt-8 text-center px-10 space-y-2">
                    <NuxtLink to="/" class="text-green-600 font-semibold text-lg">UP TO 63%</NuxtLink>
                    <NuxtLink to="/" class="font-extrabold text-3xl -tracking-wider">LogoIpsum Hosting Coupon: Save 66% +
                        Free Domain</NuxtLink>
                </div>
                <div v-if="$route.path !== '/'">
                    <div class="w-full flex items-center justify-center mt-10">
                        <button class="text-white px-10 py-4 tracking-wider rounded-md bg-lime-600 hover:bg-lime-500">GET
                            NOW</button>
                    </div>
                    <div class="flex items-center mt-5 justify-center">
                        <button class="text-slate-500 tracking-wide">READ MORE</button>
                    </div>
                </div>
            </div>
        </div>
        <div v-if="$route.path === '/'" class="flex justify-center mt-24">
            <button class=" flex bg-green-500 text-white text-lg tracking-wider px-7 py-2 rounded">VIEW ALL DEALS</button>
        </div>
    </div>
</template>