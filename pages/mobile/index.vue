<template>
  <hr />
  <Header2 />
  <hr />

  <section class="bg-[#eff6ff] h-[2090px]">

    <div class="container mx-auto">

      <div class="flex gap-[10px] text-[#8B96A5] text-[20px] pt-[25px]">
        <p>Home</p>
        <img src="../../public/icons/right.svg" alt="" />
        <p class="ml-[6px]">Clothings</p>
        <img src="../../public/icons/right.svg" alt="" />
        <p class="ml-[6px]">Men's wear</p>
        <img src="../../public/icons/right.svg" alt="" />
        <p class="ml-[6px]">Summer clothing</p>
      </div>

      <div class="flex mt-[20px] w-full">
        <Sidebar />



        <div class="ml-[21px] w-full">
          <div class="rounded-[6px] pl-[21px] border bg-white h-[70px] text-[18px] flex justify-between items-center">
            <h1>12,911 items in <strong>Mobile accessory</strong></h1>
            <div class="flex items-center">
              <p class="mr-[14px] w-[25px] h-[25px] border-[4px] rounded-[5px] border-[#BDBDBD]"></p>
              <p>Verified only</p>
              <button
                class="ml-[21px] mr-[14px] flex items-center justify-between border w-[180px] h-[42px] rounded-[6px] pr-[16px] pl-[10px]">
                Featured <img src="../../public/icons/down.svg" alt="" />
              </button>
              <p class="rounded-l-[6px] bg-[#DEE2E7] flex items-center border justify-center h-[42px] w-[40px]">
                <img class="w-[21px] h-[21px]" src="../../public/icons/kubik.svg" alt="" />
              </p>
              <p class="rounded-r-[6px] flex items-center border justify-center h-[42px] w-[40px] mr-[13px]">
                <img class="w-[22px] h-[22px]" src="../../public/icons/menu.svg" alt="" />
              </p>
            </div>
          </div>


          <div class="flex mt-[25px] gap-[15px]">
            <div v-for="el in PhoneModelsLinks" class="">
              <button
                class="text-[19px] text-[#505050] rounded-[5px] pl-[10px] pr-[20px] flex items-center justify-center border-[2px] border-[#0D6EFD] h-[40px] bg-white">
                {{ el.name }}
                <img class="ml-[30px] mr-[-10px]" src="../../public/icons/iks.svg" alt="" />
              </button>

            </div>

            <p class="text-[18px] flex items-center ml-[20px] text-[#0D6EFD]">
              Clear all filter
            </p>
          </div>

          <div class="flex w-full mt-[20px] gap-[30px]">
            <div class="w-[810px]  grid grid-cols-2 gap-[30px]">
              <div class="w-full bg-white rounded-[8px] h-[490px] border-[2px]" v-for="el in  GadgetsLinks2 ">
                <div class="flex justify-center">
                  <img class="w-[240px] h-[240px] mt-[30px] mb-[35px]" :src="`/images/${el.img}`" alt="" />
                </div>
                <hr />
                <div class="flex mt-[21px] justify-between pl-[21px]">
                  <div>
                    <img class="w-[180px]" :src="`/icons/${el.price}`" alt="" />
                    <img class="mt-[12px] w-[150px]" :src="`/icons/${el.rating}`" alt="" />
                  </div>
                  <div class="mr-[21px] w-[55px] h-[55px] border flex items-center justify-center rounded-[8px]">
                    <img src="../../public/icons/blueHeart.svg" alt="" />
                  </div>
                </div>
                <p class="mt-[15px] mb-[18pxgap-[30px]] ml-[20px] text-[#606060] text-[20px] w-[250px]">GoPro HERO6 4K
                  Action<br>Camera - Black</p>
              </div>
            </div>


<div class="w-1/3  grid grid-cols-1 gap-[30px]">
              <div class="w-[383px] bg-white rounded-[8px] border-[2px]" v-for=" el  in  GadgetsLinks ">
                <div class="flex justify-center">
                  <img class="w-[240px] h-[240px] mt-[30px] mb-[35px]" :src="`/images/${el.img}`" alt="" />
                </div>
                <hr />

                <div class="flex mt-[21px] justify-between pl-[20px]">
                  <div>
                    <img class="w-[85px]" :src="`/icons/${el.price}`" alt="" />
                    <img class="mt-[12px] w-[150px]" :src="`/icons/${el.rating}`" alt="" />
                  </div>
                  <div class="mr-[20px] w-[55px] h-[55px] border flex items-center justify-center rounded-[8px]">
                    <img src="../../public/icons/blueHeart.svg" alt="" />
                  </div>
                </div>
                <p class="mt-[15px] mb-[18px] ml-[20px] text-[#606060] text-[20px] w-[250px] ">GoPro HERO6 4K
                  Action<br>Camera - Black</p>
              </div>
            </div>
          </div>

          <div class="flex justify-end gap-5 py-5 mt-[20px] text-end pr-3">
            <div class="bg-none px-2 py-2 border-none border-gray-300 rounded-lg text-[18px]">
              <select
                class="border-[2px] border-gray-300 w-[160px] h-[50px] text-[20px] rounded-md cursor-pointer bg-white outline-none pr-5 text-gray-800">
                <option>Show 10</option>
                <option>Show 10-20</option>
                <option>Show 20-30</option>
              </select>
            </div>
            
            <ul class="flex items-center gap-0 rounded-lg text-[18px] mr-[-10px]">
              <li class="px-2 p-1cursor-pointer border-r rounded-l-lg">
              <li
                class="w-[60px] h-[50px] border-[2px] flex items-center justify-center bg-white rounded-l-md border-gray-300 mr-[-10px]">
                <img src="../../public/icons/left.svg" alt="">
              </li>
              </li>
              <li v-for="i in 3"
                class="hover:text-gray-400 w-[60px] h-[50px] border-[2px] border-gray-300 text-[22px] flex items-center justify-center bg-white hover:bg-gray-100 cursor-pointer border-r">
                {{ i }}
              </li>
              <li class="px-2 p-1 border-none cursor-pointer border-r rounded-r-lg">
              <li
                class="w-[60px] h-[50px] border-[2px] flex items-center justify-center bg-white rounded-r-md border-gray-300 ml-[-10px] hover:bg-gray-100">
                <img src="../../public/icons/right2.svg" alt="">
              </li>
              </li>
            </ul>
          </div>
        </div>
      </div>
    </div>
  </section>

  <Footer2 />
</template>

<script setup>
const PhoneModelsLinks = [
  {
    name: "Samsung"
  },
  {
    name: "Apple"
  },
  {
    name: "Poco"
  },
  {
    name: "Metallic"
  },
  {
    name: "4 star"
  },
  {
    name: "3 star"
  },
]

const GadgetsLinks = [
  {
    id: 1,
    img: "canonCamera.png",
    price: "price.svg",
    rating: "rating7_5.svg",
  },
  {
    id: 2,
    img: "iphoneBlue2.png",
    price: "price.svg",
    rating: "rating7_5.svg",
  },
  {
    id: 3,
    img: "iphone.png",
    price: "price.svg",
    rating: "rating7_5.svg",
  }
]

const GadgetsLinks2 = [
  {
    id: 1,
    img: "iphone.png",
    price: "bigPrice.svg",
    rating: "rating7_5.svg",
  },
  {
    id: 2,
    img: "iphoneBlue2.png",
    price: "bigPrice.svg",
    rating: "rating5_9.svg",
  },
  {
    id: 3,
    img: "planshet.png",
    price: "bigPrice.svg",
    rating: "rating7_5.svg",
  },
  {
    id: 4,
    img: "goProCamera.png",
    price: "bigPrice.svg",
    rating: "rating7_5.svg",
  },
  {
    id: 5,
    img: "laptop.png",
    price: "bigPrice.svg",
    rating: "rating7_5.svg",
  },
  {
    id: 6,
    img: "smartWatches.png",
    price: "bigPrice.svg",
    rating: "rating7_5.svg",
  },
]
</script>

<style lang="scss" scoped></style>