<template>
    <header class="bg-[#163300] text-white lg:pb-0">
        <div class="mx-auto w-[90%] max-w-[1700px]">
            <nav class="flex items-center justify-between h-16 lg:h-20">
                <div class="flex-shrink-0">
                    <a href="#" title="" class="flex">
                        <img
                            class="w-auto h-8 lg:h-10"
                            src="../assets/finto-logo.svg"
                            alt=""
                        />
                    </a>
                </div>

                <button
                    type="button"
                    class="inline-flex p-2 text-black transition-all duration-200 rounded-md lg:hidden focus:bg-gray-100 hover:bg-gray-100"
                    @click="toggleMenu"
                >
                    <svg
                        class="block w-6 h-6"
                        xmlns="http://www.w3.org/2000/svg"
                        fill="none"
                        viewBox="0 0 24 24"
                        stroke="currentColor"
                    >
                        <path
                            stroke-linecap="round"
                            stroke-linejoin="round"
                            stroke-width="2"
                            d="M4 8h16M4 16h16"
                        />
                    </svg>

                    <svg
                        class="hidden w-6 h-6"
                        xmlns="http://www.w3.org/2000/svg"
                        fill="none"
                        viewBox="0 0 24 24"
                        stroke="currentColor"
                    >
                        <path
                            stroke-linecap="round"
                            stroke-linejoin="round"
                            stroke-width="2"
                            d="M6 18L18 6M6 6l12 12"
                        />
                    </svg>
                </button>
                <div
                    class="hidden lg:w-[60%] xl:w-[65%] lg:flex lg:items-center text-xl lg:ml-auto lg:space-x-10"
                >
                    <a href="#" title="" class="text-base"> Features </a>

                    <a href="#" title="" class="text-base"> Solutions </a>

                    <a href="#" title="" class="text-base"> Customers </a>

                    <a href="#" title="" class="text-base"> Resources </a>

                    <a href="#" title="" class="text-base"> Pricings </a>
                </div>

                <a href="#" title="" class="text-xl hidden lg:inline-flex">
                    Login
                </a>
                <a
                    href="#"
                    title=""
                    class="items-center justify-center hidden px-6 py-2 ml-10 text-xl font-semibold text-black transition-all duration-200 bg-[#9FE870] border border-transparent rounded-full lg:inline-flex hover:[#9FE870] focus:[#9FE870]"
                    role="button"
                >
                    Signup
                </a>
            </nav>

            <nav
                class="pt-4 pb-6 bg-white border border-gray-200 text-black rounded-md shadow-md lg:hidden"
                :class="{ hidden: !menuOpen }"
            >
                <div class="flow-root">
                    <div class="flex flex-col px-6 -my-2 space-y-4">
                        <a href="#" title="" class="text-base"> Features </a>

                        <a href="#" title="" class="text-base"> Solutions </a>

                        <a href="#" title="" class="text-base"> Customers </a>

                        <a href="#" title="" class="text-base"> Resources </a>

                        <a href="#" title="" class="text-base"> Pricings </a>
                    </div>
                </div>

                <div class="px-6 mt-6 flex space-y-4 flex-col">
                    <a href="#" title="" class=""> Login </a>
                    <a
                        href="#"
                        title=""
                        class="items-center justify-center px-6 py-2 font-semibold text-black transition-all duration-200 bg-[#9FE870] border border-transparent rounded-full lg:inline-flex hover:[#9FE870] focus:[#9FE870]"
                        role="button"
                    >
                        Signup
                    </a>
                </div>
            </nav>
        </div>
    </header>
</template>

<script lang="ts">
export default {
    data() {
        return {
            menuOpen: false,
        };
    },

    methods: {
        toggleMenu() {
            this.menuOpen = !this.menuOpen;
        },
    },
};
</script>
