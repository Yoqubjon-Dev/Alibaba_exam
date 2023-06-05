<template>


    <div class="container mx-auto w-screen h-24 flex flex-col justify-center">
        <select
            class="absolute ml-[844px] pr-12 pl-6  text-[21px] text-black max-w-fit leading-tight focus:outline-none pt-3 pb-3 border-[#0D6EFD] rounded-none"
            name="select" id="select">
            <option value="1">All category</option>
            <option value="2">Category 2</option>
            <option value="3">Mobile</option>
        </select>

        <div class="flex items-center justify-between gap-12">
            <img class="p-4 w-52" src="../public/images/logo.png" alt="">

            <div class="flex rounded-xl bg-white border-[3px] border-[#0D6EFD] w-[900px] h-14 items-center justify-end">
                <i class="text-[25px] text-[#AAAAAA]"></i>
                <input class="rounded-l-xl w-full h-full outline-none border-none" type="text" placeholder="Search">
                <button class="w-2/6 h-14 flex items-center text-center border-[3px] border-[#0D6EFD]">
                </button>
                <button class="rounded-r-md bg-[#0D6EFD] w-1/4 h-full flex items-center text-center">
                    <p class="text-white ml-[34px] text-[21px]">Search</p>
                </button>
            </div>
            <div class="flex gap-[25px] text-[#8B96A5]">
                <div class="flex flex-col items-center mt-4">
                    <img class="w-[26px]" src="../public/icons/profile.svg" alt="">
                    <p>Profile</p>
                </div>
                <div class="flex flex-col items-center mt-4">
                    <img class="w-[26px]" src="../public/icons/message.svg" alt="">
                    <p>Message</p>
                </div>
                <div class="flex flex-col items-center mt-4">
                    <img class="w-[26px]" src="../public/icons/orders.svg" alt="">
                    <p class="mt-1">Orders</p>
                </div>
                <div class="flex flex-col items-center mt-4">
                    <NuxtLink to="/my-cart" class="flex flex-col items-center">
                        <img class="w-[26px]" src="../public/icons/mycart.svg" alt="">
                        <p>My cart</p>
                    </NuxtLink>
                </div>
            </div>
        </div>
    </div>
</template>


<script setup>

</script>

<style lang="scss" scoped></style>