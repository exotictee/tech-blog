<template>
    <section class="bg-gray-100">
        <div class="bg-purple h-[40vh] relative object-cover object-center bg-no-repeat">
            <navbar :page="'index'" />
            <div class="absolute flex items-center justify-center w-full bottom-10">
                <h1 class="text-white font-extrabold text-7xl tracking-wider pb-6">Contact</h1>
            </div>
        </div>
        <div class="flex flex-col items-center space-y-6 mt-20">
            <h1 class="text-5xl tracking-wide font-extrabold">WANT TO GET IN TOUCH?</h1>
            <h3 class="text-2xl tracking-wide font-extrabold">Use this contact form below. We typically reply within 24
                hours.
            </h3>
        </div>
        <div class="-mt-16">
            <VertLine />
        </div>
        <div class="flex px-64 mt-24">
            <form action="" class="w-full bg-white shadow-xl p-16 rounded-md mb-20">
                <div class="flex flex-col w-full">
                    <label for="full_name" class="relative text-xl font-bold">
                        Name
                        <sup class="text-red-500 text-lg">*</sup>
                    </label>
                    <div class="flex flex-row w-full space-x-4">
                        <div class="flex flex-col w-1/2">
                            <input type="text" id="first_name" class="border border-gray-400 p-4 rounded-sm w-full">
                            <span class="text-gray-500 text-sm">First</span>
                        </div>
                        <div class="flex flex-col w-1/2">
                            <input type="text" id="last_name" class="border border-gray-400 p-4 rounded-sm w-full">
                            <span class="text-gray-500 text-sm">Last</span>
                        </div>
                    </div>
                </div>
                <div class="flex flex-col w-full mt-14">
                    <label for="email" class="relative text-xl font-bold">
                        Email
                        <sup class="text-red-500 text-lg">*</sup>
                    </label>
                    <input type="email" class="w-full border border-gray-400 rounded-sm p-4">
                </div>

                <div class="flex flex-col w-full mt-14">
                    <label for="email" class="relative text-xl font-bold">
                        Message
                        <sup class="text-red-500 text-lg">*</sup>
                    </label>
                    <textarea id="message" class="border border-gray-400 rounded-md p-2 mt-2" rows="6"></textarea>
                </div>

                <div class="mt-10">
                    <button class="px-6 py-2 text-white bg-lime-600 text-lg">SUBMIT</button>
                </div>
            </form>
        </div>


        <div class="bg-purple min-h-screen object-cover object-center bg-no-repeat">
            <Footer />
        </div>
    </section>
</template>