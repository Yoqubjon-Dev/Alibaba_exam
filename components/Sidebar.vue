
<template>
    <div class="mt-[5px] w-[400px]">
        <div id="accordion-open" class="w-full" data-accordion="open">
            <hr>
            <h2 id="accordion-open-heading-1">
                <button type="button"
                    class="text-[18px] flex items-center justify-between w-full p-5 font-medium text-left text-gray-500 focus:ring-0 border-none"
                    data-accordion-target="#accordion-open-body-1" aria-expanded="true"
                    aria-controls="accordion-open-body-1">
                    Category
                    <svg data-accordion-icon class="w-6 h-6 rotate-180 shrink-0" fill="currentColor" viewBox="0 0 20 20"
                        xmlns="http://www.w3.org/2000/svg">
                        <path fill-rule="evenodd"
                            d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                            clip-rule="evenodd"></path>
                    </svg>
                </button>
            </h2>
            <div id="accordion-open-body-1" class="hidden" aria-labelledby="accordion-open-heading-1">
                <div class="pl-5 grid grid-cols-1 text-[#505050] text-[18px]">
                    <h1 v-for="el in Categories"
                        class="w-full py-[10px] hover:cursor-pointer duration-300 hover:text-black">
                        {{ el.title }}
                    </h1>
                    <h1 class="w-full py-[10px] hover:cursor-pointer duration-300 hover:text-[#144184] text-[#0D6EFD]">
                        See all
                    </h1>
                </div>
            </div>
            <hr>
            <h2 id="accordion-open-heading-2">
                <button type="button"
                    class="flex items-center justify-between w-full p-5 text-[18px] font-medium text-left text-gray-500 focus:ring-0 border-none"
                    data-accordion-target="#accordion-open-body-2" aria-expanded="false"
                    aria-controls="accordion-open-body-2">
                    Brands
                    <svg data-accordion-icon class="w-6 h-6 shrink-0" fill="currentColor" viewBox="0 0 20 20"
                        xmlns="http://www.w3.org/2000/svg">
                        <path fill-rule="evenodd"
                            d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                            clip-rule="evenodd"></path>
                    </svg>
                </button>
            </h2>
            <div id="accordion-open-body-2" class="hidden" aria-labelledby="accordion-open-heading-2">
                <div class="pl-5">
                    <div class="grid grid-cols-1 text-[#505050] text-[18px]">
                        <div v-for="el in Brands" class="flex py-[10px] items-center justify-start gap-3">
                            <input class="border-[2px] border-gray-400 rounded-[6px] w-[20px] h-[20px] hover:cursor-pointer"
                                type="checkbox" :title="el" />
                            <h1 :for="el" class="w-full">{{ el.title }}</h1>
                        </div>
                        <h1 class="w-full py-[10px] hover:cursor-pointer duration-300 hover:text-[#144184] text-[#0D6EFD]">
                            See all
                        </h1>
                    </div>
                </div>
            </div>
            <hr>
            <h2 id="accordion-open-heading-3">
                <button type="button"
                    class="text-[18px] flex items-center justify-between w-full p-5 font-medium text-left text-gray-500 focus:ring-0 border-none"
                    data-accordion-target="#accordion-open-body-3" aria-expanded="false"
                    aria-controls="accordion-open-body-3">
                    Features
                    <svg data-accordion-icon class="w-6 h-6 shrink-0" fill="currentColor" viewBox="0 0 20 20"
                        xmlns="http://www.w3.org/2000/svg">

<path fill-rule="evenodd"
                            d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                            clip-rule="evenodd"></path>
                    </svg>
                </button>
            </h2>
            <div id="accordion-open-body-3" class="hidden" aria-labelledby="accordion-open-heading-3">
                <div class="pl-5">
                    <div class="grid grid-cols-1 text-[#505050] text-[18px]">
                        <div v-for="el in Features" class="flex py-[10px] items-center justify-start gap-3">
                            <input class="border-[2px] border-gray-400 rounded-[6px] w-[20px] h-[20px] hover:cursor-pointer"
                                type="checkbox" :title="el" />
                            <h1 :for="el" class="w-full">{{ el.title }}</h1>
                        </div>
                        <h1 class="w-full py-[10px] hover:cursor-pointer duration-300 hover:text-[#144184] text-[#0D6EFD]">
                            See all
                        </h1>
                    </div>
                </div>
            </div>
            <hr>
            <h2 id="accordion-open-heading-4">
                <button type="button"
                    class="text-[18px] flex items-center justify-between w-full p-5 font-medium text-left text-gray-500 focus:ring-0 border-none bg-none"
                    data-accordion-target="#accordion-open-body-4" aria-expanded="false"
                    aria-controls="accordion-open-body-4">
                    Price range
                    <svg data-accordion-icon class="w-6 h-6 shrink-0" fill="currentColor" viewBox="0 0 20 20"
                        xmlns="http://www.w3.org/2000/svg">
                        <path fill-rule="evenodd"
                            d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                            clip-rule="evenodd"></path>
                    </svg>
                </button>
            </h2>
            <div id="accordion-open-body-4" class="hidden" aria-labelledby="accordion-open-heading-4">
                <div class="pl-5">
                    <div class="grid grid-cols-1 text-[#505050] text-[18px]">
                        <div v-for="el in PriceRange" class="flex py-[10px] items-center justify-start gap-3">
                            <input class="border-[2px] border-gray-400 rounded-[6px] w-[20px] h-[20px] hover:cursor-pointer"
                                type="checkbox" :title="el" />
                            <h1 :for="el" class="w-full">{{ el.title }}</h1>
                        </div>
                        <h1 class="w-full py-[10px] hover:cursor-pointer duration-300 hover:text-[#144184] text-[#0D6EFD]">
                            See all
                        </h1>
                    </div>
                </div>
            </div>
            <hr>
            <h2 id="accordion-open-heading-5">
                <button type="button"
                    class="text-[18px] flex items-center justify-between w-full p-5 font-medium text-left text-gray-500 focus:ring-0 border-none"
                    data-accordion-target="#accordion-open-body-5" aria-expanded="false"
                    aria-controls="accordion-open-body-5">
                    Condition
                    <svg data-accordion-icon class="w-6 h-6 shrink-0" fill="currentColor" viewBox="0 0 20 20"
                        xmlns="http://www.w3.org/2000/svg">
                        <path fill-rule="evenodd"
                            d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                            clip-rule="evenodd"></path>
                    </svg>
                </button>
            </h2>
            <div id="accordion-open-body-5" class="hidden" aria-labelledby="accordion-open-heading-5">
                <div class="pl-5">

<div class="grid grid-cols-1 text-[#505050] text-[18px]">
                        <div v-for="el in Condition" class="flex py-[10px] items-center justify-start gap-3">
                            <input class="border-[2px] border-gray-400 rounded-[6px] w-[20px] h-[20px] hover:cursor-pointer"
                                type="checkbox" :title="el" />
                            <h1 :for="el" class="w-full">{{ el.title }}</h1>
                        </div>
                        <h1 class="w-full py-[10px] hover:cursor-pointer duration-300 hover:text-[#144184] text-[#0D6EFD]">
                            See all
                        </h1>
                    </div>
                </div>
            </div>
            <hr>
            <h2 id="accordion-open-heading-6">
                <button type="button"
                    class="text-[18px] flex items-center justify-between w-full p-5 font-medium text-left text-gray-500 focus:ring-0 border-none"
                    data-accordion-target="#accordion-open-body-6" aria-expanded="false"
                    aria-controls="accordion-open-body-6">
                    Ratings
                    <svg data-accordion-icon class="w-6 h-6 shrink-0" fill="currentColor" viewBox="0 0 20 20"
                        xmlns="http://www.w3.org/2000/svg">
                        <path fill-rule="evenodd"
                            d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                            clip-rule="evenodd"></path>
                    </svg>
                </button>
            </h2>
            <div id="accordion-open-body-6" class="hidden" aria-labelledby="accordion-open-heading-6">
                <div class="pl-5">
                    <div class="grid grid-cols-1 text-[#505050] text-[18px]">
                        <div v-for="el in Ratings" class="flex py-[10px] items-center justify-start gap-3">
                            <input class="border-[2px] border-gray-400 rounded-[6px] w-[20px] h-[20px] hover:cursor-pointer"
                                type="checkbox" :title="el" />
                            <h1 :for="el" class="w-full">{{ el.title }}</h1>
                        </div>
                        <h1 class="w-full py-[10px] hover:cursor-pointer duration-300 hover:text-[#144184] text-[#0D6EFD]">
                            See all
                        </h1>
                    </div>
                </div>
            </div>
            <hr>
            <h2 id="accordion-open-heading-7">
                <button type="button"
                    class="text-[18px] flex items-center justify-between w-full p-5 font-medium text-left text-gray-500 focus:ring-0 border-none"
                    data-accordion-target="#accordion-open-body-7" aria-expanded="false"
                    aria-controls="accordion-open-body-7">
                    Manufacturer
                    <svg data-accordion-icon class="w-6 h-6 shrink-0" fill="currentColor" viewBox="0 0 20 20"
                        xmlns="http://www.w3.org/2000/svg">
                        <path fill-rule="evenodd"
                            d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                            clip-rule="evenodd"></path>
                    </svg>
                </button>
            </h2>
            <div id="accordion-open-body-7" class="hidden" aria-labelledby="accordion-open-heading-7">
                <div class="pl-5">
                    <div class="grid grid-cols-1 text-[#505050] text-[18px]">
                        <div v-for="el in Manufacturers" class="flex py-[10px] items-center justify-start gap-3">
                            <input class="border-[2px] border-gray-400 rounded-[6px] w-[20px] h-[20px] hover:cursor-pointer"
                                type="checkbox" :title="el" />
                            <h1 :for="el" class="w-full">{{ el.title }}</h1>
                        </div>

<h1 class="w-full py-[10px] hover:cursor-pointer duration-300 hover:text-[#144184] text-[#0D6EFD]">
                            See all
                        </h1>
                    </div>
                </div>
            </div>
            <hr>
        </div>
    </div>
</template>

<script setup>
import { initAccordions } from "flowbite";
import { onMounted } from "vue";

onMounted(() => {
    initAccordions();
});

const Categories = [
    {
        id: 1,
        title: "Mobile accessory"
    },
    {
        id: 2,
        title: "Electronics"
    },
    {
        id: 3,
        title: "Smartphones"
    },
    {
        title: "Modern tech"
    }
]

const Brands = [
    {
        title: "Samsung"
    },
    {
        title: "Apple"
    },
    {
        title: "Huawei"
    },
    {
        title: "Pocco"
    },
    {
        title: "Lenovo"
    }
]

const Features = [
    {
        title: "Metallic"
    },
    {
        title: "Plastic Cover"
    },
    {
        title: "8GB Ram"
    },
    {
        title: "Super power"
    },
    {
        title: "Large memory"
    }
]

const PriceRange = [
    {
        title: "0-100"
    },
    {
        title: "100-1000"
    },
    {
        title: "1000-1000"
    }
]

const Condition = [
    {
        title: "New"
    },
    {
        title: "Normal"
    },
    {
        title: "Old"
    },
    {
        title: "Unusable"
    }
]

const Ratings = [
    {
        title: "Best"
    },
    {
        title: "Medium"
    },
    {
        title: "Worst"
    }
]

const Manufacturers = [
    {
        title: "Nokia"
    },
    {
        title: "Samsung"
    },
    {
        title: "Apple"
    }
]
</script>

<style lang="scss" scoped></style>