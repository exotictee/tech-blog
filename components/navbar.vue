<script >
//    defineProps({
//             page: String
//         });

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
    props: {
        page: String
    }


};
</script>


<template>
    <div class="flex px-20 pt-10">
        <div class="flex flex-row w-full justify-between items-center">
            <div>
                <!-- Use v-if and v-else to conditionally render the logo -->
                <nuxt-link v-if="page === 'index'" to="/">
                    <img src="../assets/img/logo-regular-free-img.png" class="h-10" alt="">
                </nuxt-link>
                <nuxt-link v-else to="/">
                    <img src="../assets/img/site-logo.png" class="h-10" alt="">
                </nuxt-link>
            </div>

            <div class="space-x-8">
                <nuxt-link :class="{
                    'text-slate-200 text-xl hover:text-white': $route.path !== '/programming',
                    'text-black': $route.path === '/programming',
                    'hover:text-green-500': $route.path === '/programming',
                }" to="/">Home</nuxt-link>

                <div class="relative inline-block" @mouseenter="openArticleDropdown" @mouseleave="closeArticleDropdown">
                    <div class="flex items-center justify-center space-x-4">
                        <nuxt-link :class="{
                            'text-slate-200 text-xl hover:text-white': $route.path !== '/programming',
                            'text-black': $route.path === '/programming',
                            'hover:text-green-500': $route.path === '/programming',
                        }">
                            <span class="cursor-pointer" @mouseenter="openArticleDropdown">Article</span>
                            <i class="bx bx-chevron-down"></i>
                        </nuxt-link>
                    </div>
                    <!-- Dropdown Menu -->
                    <div v-if="isArticleDropdownOpen" class="absolute left-0 mt-2 bg-white text-black rounded-lg shadow"
                        @mouseenter="keepArticleDropdownOpen" @mouseleave="closeArticleDropdown">
                        <!-- Dropdown Links -->
                        <nuxt-link :class="{
                            'block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white':
                                $route.path === '/programming',
                            'block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white':
                                $route.path !== '/programming',
                        }" to="/programming">
                            Programming
                        </nuxt-link>
                        <nuxt-link :class="{
                            'block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white':
                                $route.path === '/programming',
                            'block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white':
                                $route.path !== '/programming',
                        }" to="/cryptocurrency">
                            Cryptocurrency
                        </nuxt-link>
                        <nuxt-link :class="{
                            'block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white':
                                $route.path === '/programming',
                            'block px-4 py-2 hover:bg-gray-100 dark:hover:bg-gray-600 dark:hover:text-white':
                                $route.path !== '/programming',
                        }" to="/technologies">
                            Technologies
                        </nuxt-link>
                    </div>
                </div>
                <nuxt-link :class="{
                    'text-slate-200 text-xl hover:text-white': $route.path !== '/programming',
                    'text-black': $route.path === '/programming',
                    'hover:text-green-500': $route.path === '/programming',
                }" to="/deals">Deals</nuxt-link>
                <nuxt-link :class="{
                    'text-slate-200 text-xl hover:text-white': $route.path !== '/programming',
                    'text-black': $route.path === '/programming',
                    'hover:text-green-500': $route.path === '/programming',
                }" to="/about">About</nuxt-link>
                <nuxt-link :class="{
                    'text-slate-200 text-xl hover:text-white': $route.path !== '/programming',
                    'text-black': $route.path === '/programming',
                    'hover:text-green-500': $route.path === '/programming',
                }" to="/contact">Contact</nuxt-link>
                <nuxt-link :class="{
                    'text-slate-200 text-xl hover:text-white': $route.path !== '/programming',
                    'text-black': $route.path === '/programming',
                    'hover:text-green-500': $route.path === '/programming',
                }" to="/search"><i class="bx bx-search"></i></nuxt-link>
            </div>
        </div>
    </div>
</template>
  

  