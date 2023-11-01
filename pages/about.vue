<template>
    <div class="bg-purple h-[40vh] relative object-cover object-center bg-no-repeat">
        <navbar :page="'index'" />
        <div class="absolute flex items-center justify-center w-full bottom-10">
            <h1 class="text-white font-extrabold text-7xl tracking-wider pb-6">About</h1>
        </div>
    </div>
    <div>
        <VertLine />
    </div>
    <div class="relative h-[250vh]">
        <h1 class="font-extrabold text-5xl text-center pt-14">ABOUT JUSTIN BARRETT</h1>
        <div class="flex relative flex-row justify-between  px-20 w-full">
            <div class="w-2/5 flex flex-col pt-36">
                <p class="font-extrabold text-3xl tracking-wide">Hey Technology Enthusiast,</p>
                <p class="font-extrabold text-xl mt-8 tracking-wider">Incididunt ut labore et dolore magna aliqua. Ut enim
                    ad
                    ut
                    aliquip ex ea commodo consequat. Duis aute irure
                    dolor in reprehenderit.
                </p>
                <p class="text-xl mt-8 text-gray-700">Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do
                    eiusmod
                    tempor incididunt ut labore et
                    dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip
                    ex
                    ea commodo consequat. Duis aute irure dolor in reprehenderit
                </p>
                <p class="text-xl mt-14 text-gray-700">Incididunt ut labore et dolore magna aliqua. Ut enim ad ut aliquip ex
                    ea
                    commodo consequat. Duis aute irure
                    dolor in reprehenderit.
                </p>
            </div>
            <div class="mt-20 w-[50%]">
                <img src="../assets/img/teaching.jpg" class="w-full" alt="">
            </div>
        </div>

        <BlogContent />

    </div>
    <SlideLogo />
    <div class="bg-purple min-h-screen object-cover object-center bg-no-repeat">
        <Footer />
    </div>
</template>