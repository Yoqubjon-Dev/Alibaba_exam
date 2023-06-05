<template>


    <div class="container mx-auto w-screen h-24 flex flex-col justify-center">
        <div class="flex items-center justify-between gap-12">
            <img class="p-4 w-52" src="../public/images/logo.png" alt="">

            <div class="flex gap-[26px] text-[#8B96A5]">
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