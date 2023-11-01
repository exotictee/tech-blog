<template>
    <div class="bg-purple h-[40vh] relative object-cover object-center bg-no-repeat">
        <navbar :page="'index'" />
        <div class="absolute flex items-center justify-center w-full bottom-10">
            <h1 class="text-white font-extrabold text-7xl tracking-wider pb-6">Deals</h1>
        </div>
    </div>
    <div class="bg-white">
        <LogoCard />
    </div>
    <div>
        <hr class="w-full my-2 sm:my-4 md:my-6 lg:my-8 bg-gray-200">
    </div>
    <div class="bg-white">
        <Logocard2 />
    </div>
    <div>
        <hr class="w-full my-2 sm:my-4 md:my-6 lg:my-8 bg-gray-200">
    </div>
    <div class="mt-44">
        <SlideLogo />
    </div>
    <div class="bg-purple min-h-screen object-cover object-center bg-no-repeat">
        <Footer />
    </div>
</template>