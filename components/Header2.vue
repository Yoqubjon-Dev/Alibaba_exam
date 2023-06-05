<template>


    <div class="container mx-auto">
        <select
            class="absolute ml-[1160px] border-none text-[24px] text-black rounded-md max-w-fit leading-tight focus:outline-none mt-[-5px]"
            name="select" id="select">
            <option value="1">English, USD</option>
            <option value="2">Russian, RUB</option>
            <option value="3">Uzbek, UZS</option>
        </select>

        <select
            class="absolute ml-[698px] w-[106px] border-none text-[24px] text-black rounded-md max-w-fit leading-tight focus:outline-none mt-[-5px]"
            name="select" id="select">
            <option value="1">Help</option>
            <option value="2">Word1</option>
            <option value="3">Word2</option>
        </select>

        <div class="absolute ml-[1375px] mt-[-5px] flex items-center">
            <img class="absolute h-[24px] ml-[90px]" src="../public/images/germany.png" alt="">
            <select
                class="border-none text-[22px] text-black rounded-md max-w-fit leading-tight focus:outline-none"
                name="select" id="select">
                <option value="1">Ship toㅤㅤ</option>
                <option value="2">Ship toㅤㅤ</option>
                <option value="3">Ship toㅤㅤ</option>
            </select>
        </div>

        <nav class="mt-[18px] mb-[18px] flex justify-between">
            <div class="flex gap-[28px] text-[24px]">
                <img src="../public/icons/menu.svg" alt="">
                <h1 class="ml-[-15px]">All category</h1>
                <h1>Hot offers</h1>
                <h1>Gift boxes</h1>
                <h1>Projects</h1>
                <h1>Menu item</h1>
            </div>
            <div class="flex gap-[32px] text-[22px]">
            </div>
        </nav>
    </div>
</template>


<script setup>

</script>

<style lang="scss" scoped></style>