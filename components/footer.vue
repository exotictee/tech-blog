<script>
export default {
    data() {
        return {
            email: '',
            showMessage: false,
        };
    },
    computed: {
        isIndexPage() {
            // Check if the current route is the index page ("/" or "/index")
            return this.$route.path === '/' || this.$route.path === '/index';
        },
    },
    methods: {
        submitForm() {
            if (this.isValidEmail(this.email)) {
                // Set showMessage to true to display the thank you message and hide the form
                this.showMessage = true;
            } else {
                alert("Please enter a valid email address.");
            }
        },
        isValidEmail(email) {
            // Use a regular expression to check if the email is in a valid format
            const emailRegex = /^[a-zA-Z0-9._-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,4}$/;
            return emailRegex.test(email);
        },
    },
};
</script>

<template>
    <div class="pt-20">
        <div class="flex px-20 flex-row justify-between w-full">
            <div class="flex flex-col space-y-7 text-white">
                <h2 class="text-2xl font-bold tracking-wider">FOLLOW US</h2>
                <p class="text-lg">Lorem ipsum dolor sit amet, consectetur</p>
                <div class="flex flex-row space-x-7 text-5xl">
                    <NuxtLink to="/" class="hover:opacity-40"><i class='bx bxl-facebook-circle'></i></NuxtLink>
                    <NuxtLink to="/" class="hover:opacity-40"><i class='bx bxl-twitter'></i></NuxtLink>
                    <NuxtLink to="/" class="hover:opacity-40"><i class='bx bxl-instagram'></i></NuxtLink>
                </div>
            </div>
            <div class="flex flex-col space-y-3 mr-28">
                <h2 class="text-white text-2xl font-bold tracking-wider">SUBSCRIBE TO OUR NEWSLETTER</h2>

                <!-- Conditionally render the content based on whether it's the index page or not -->
                <div v-if="isIndexPage">
                    <p class="text-white text-lg">Thanks for contacting us! We will be in touch with you shortly.</p>
                </div>

                <div v-else>
                    <!-- Conditionally render the email form or thank you message -->
                    <div v-if="!showMessage" class="flex flex-row pb-9 space-x-2">
                        <input v-model="email" type="text" placeholder="Email address"
                            class="bg-white w-[550px] px-5 rounded text-xl py-4" @keydown.enter="submitForm">
                        <button @click="submitForm"
                            class="bg-green-600 text-white px-14 rounded py-1 text-xl">Submit</button>
                    </div>

                    <div v-else class="flex flex-row pb-9 space-x-2">
                        <p class="flex justify-end text-slate-300 font-extrabold text-lg">Thank you for contacting us, we'll
                            get to you shortly.</p>
                    </div>
                </div>
            </div>
        </div>
        <hr class="w-full mt-20  opacity-30">
        <div class="flex flex-row px-20 w-full justify-end mt-20">
            <div class="flex flex-col space-y-7 mr-36">
                <h2 class="text-white text-2xl font-bold">LEARN</h2>
                <div class="flex flex-col space-y-1">
                    <NuxtLink to="/" class="text-white text-lg hover:opacity-40">Cryptocurrency</NuxtLink>
                    <NuxtLink to="/" class="text-white text-lg hover:opacity-40">Programming</NuxtLink>
                    <NuxtLink to="/" class="text-white text-lg hover:opacity-40">Technologies</NuxtLink>
                </div>
            </div>
            <div class="flex flex-col space-y-7">
                <h2 class="text-white text-2xl font-bold">DEALS</h2>
                <div class="flex flex-col space-y-1">
                    <NuxtLink to="/" class="text-white text-lg hover:opacity-40">IdeaFirm Hosting Coupon</NuxtLink>
                    <NuxtLink to="/" class="text-white text-lg hover:opacity-40">Pretended Company Discount Code</NuxtLink>
                    <NuxtLink to="/" class="text-white text-lg hover:opacity-40">LogoIpsum Coupon Code</NuxtLink>
                </div>
            </div>
        </div>
        <hr class="w-full mt-20  opacity-30">
        <p class="text-white opacity-40 tracking-wider text-sm py-10 px-20">Copyright © 2023 Tech Blogger | Powered by Tech
            Blogger</p>
    </div>
</template>