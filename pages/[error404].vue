<script setup></script>

<template>
    <main class="bg-[#eff6ff] h-screen flex items-center">
        <div class="container mx-auto h-[700px] flex justify-start items-start">
            <img class="ml-[100px] w-[700px] h-[700px]" src="/images/error.png" alt="" />
            <div style="font-family: sans-serif" class="ml-[57px]">
                <h1 class=" mt-[300px] text-[80px] text-green-500 font-semibold">
                    404 not found
                </h1>

                <p class="text-green-400 text-[34px] mb-[20px]">
                    Looking something we don't serve?
                </p>
                <nuxt-link to="/" class="text-green-900 text-[25px] underline">back to home</nuxt-link>
            </div>
        </div>
    </main>
</template>

<script setup>
definePageMeta({

  layout: "my-cart",

});
</script>

<style lang="scss" scoped></style>