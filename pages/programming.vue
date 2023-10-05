<template >
    <div>
        <navbar :page="'programme'" />
        <div class="mt-10 px-60 w-full h-fit bg-slate-50 py-20">
            <h1 class="text-5xl font-bold ml-14">Technologies</h1>
            <div class="flex flex-col space-y-3 pt-20 min-h-screen">
                <NuxtLink to="/" class="w-full ">
                    <img src="../assets/img/big-code.jpg" class="w-full" alt="">
                </NuxtLink>
                <NuxtLink to="/" class="w-full">
                    <h1 class="mt-10 text-4xl text-gray-950 font-extrabold tracking-wider">THE BEST CODING TRICK TO LOREM
                        IPSUM</h1>
                </NuxtLink>
                <div class="flex flex-row space-x-3 text-lg ">
                    <NuxtLink to="/" class="hover:text-lime-500">Leave a comment</NuxtLink>
                    <span>/</span>
                    <NuxtLink to="/" class="hover:text-lime-500">Programming</NuxtLink>
                </div>
                <h1>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptates qui inventore unde voluptatum quia
                    commodi laudantium! Iure corporis obcaecati repellendus odio distinctio perspiciatis, adipisci quisquam
                    officiis, quasi numquam nihil optio.
                    Facilis asperiores maxime id vitae provident earum.
                </h1>
            </div>
            <hr class="border-t-2 border-slate-300 w-full my-10">

            <div class="flex flex-col space-y-3 pt-20 min-h-screen">
                <NuxtLink to="/" class="w-full ">
                    <img src="../assets/img/big-laptop.jpg" class="w-full" alt="">
                </NuxtLink>
                <NuxtLink to="/" class="w-full">
                    <h1 class="mt-10 text-4xl text-gray-950 font-extrabold tracking-wider uppercase">How to Lorem ipsum
                        dolor sit amet, consectetur</h1>
                </NuxtLink>
                <div class="flex flex-row space-x-3 text-lg ">
                    <NuxtLink to="/" class="hover:text-lime-500">Leave a comment</NuxtLink>
                    <span>/</span>
                    <NuxtLink to="/" class="hover:text-lime-500">Programming</NuxtLink>
                </div>
                <h1>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptates qui inventore unde voluptatum quia
                    commodi laudantium! Iure corporis obcaecati repellendus odio distinctio perspiciatis, adipisci quisquam
                    officiis, quasi numquam nihil optio.
                    Facilis asperiores maxime id vitae provident earum.
                </h1>
            </div>
            <hr class="border-t-2 border-slate-300 w-full my-10">

            <div class="flex flex-col space-y-3 pt-20 min-h-screen">
                <NuxtLink to="/" class="w-full ">
                    <img src="../assets/img/big-programmer.jpg" class="w-full" alt="">
                </NuxtLink>
                <NuxtLink to="/" class="w-full">
                    <h1 class="mt-10 text-4xl text-gray-950 font-extrabold tracking-wider uppercase">Best places to
                        download html templates</h1>
                </NuxtLink>
                <div class="flex flex-row space-x-3 text-lg ">
                    <NuxtLink to="/" class="hover:text-lime-500">Leave a comment</NuxtLink>
                    <span>/</span>
                    <NuxtLink to="/" class="hover:text-lime-500">Programming</NuxtLink>
                </div>
                <h1>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptates qui inventore unde voluptatum quia
                    commodi laudantium! Iure corporis obcaecati repellendus odio distinctio perspiciatis, adipisci quisquam
                    officiis, quasi numquam nihil optio.
                    Facilis asperiores maxime id vitae provident earum.
                </h1>
            </div>
            <hr class="border-t-2 border-slate-300 w-full my-10">

        </div>
        <div class="bg-purple min-h-screen object-cover object-center bg-no-repeat">
            <Footer />
        </div>
    </div>
</template>