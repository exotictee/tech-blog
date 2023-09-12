<script>
export default {
    data() {
        return {
            isArticleDropdownOpen: false,
        };
    },
    methods: {
        openArticleDropdown() {
            this.isArticleDropdownOpen = true;
        },
        closeArticleDropdown() {
            this.isArticleDropdownOpen = false;
        },
        keepArticleDropdownOpen() {
            // Do nothing, keep the dropdown open when hovering over it.
        },
    },
};
</script>

<template>
    <div class="flex px-20 pt-10">
        <div class="flex flex-row w-full justify-between items-center">
            <div>
                <img src="../assets/img/logo-regular-free-img.png" class="h-10" alt="">
            </div>
            <div class="space-x-8">
                <nuxt-link class="text-slate-200 text-xl hover:text-white" to="/">Home</nuxt-link>

                <div class="relative inline-block" @mouseenter="openArticleDropdown" @mouseleave="closeArticleDropdown">
                    <nuxt-link class="text-slate-200 text-xl hover:text-white">
                        <span class="cursor-pointer" @mouseenter="openArticleDropdown">Article</span>
                        <i class="bx bx-chevron-down"></i>
                    </nuxt-link>
                    <!-- Dropdown Menu -->
                    <div v-if="isArticleDropdownOpen" class="absolute left-0 mt-2 bg-white text-black rounded-lg shadow"
                        @mouseenter="keepArticleDropdownOpen" @mouseleave="closeArticleDropdown">
                        <!-- Dropdown Links -->
                        <nuxt-link to="/"
                            class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">
                            Programming
                        </nuxt-link>
                        <nuxt-link to="/"
                            class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">
                            Cryptocurrency
                        </nuxt-link>
                        <nuxt-link to="/"
                            class="block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white">
                            Technologies
                        </nuxt-link>
                    </div>
                </div>
                <nuxt-link class="text-slate-200 text-xl hover:text-white" to="/">Deals</nuxt-link>
                <nuxt-link class="text-slate-200 text-xl hover:text-white" to="/">About</nuxt-link>
                <nuxt-link class="text-slate-200 text-xl hover:text-white" to="/">Contact</nuxt-link>
                <nuxt-link class="text-slate-200 text-xl hover:text-white" to="/"><i class="bx bx-search"></i></nuxt-link>
            </div>
        </div>
    </div>
</template>