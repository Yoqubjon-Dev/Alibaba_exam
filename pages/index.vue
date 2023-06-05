<template>
  <Header2 />
  <hr>
  <main class="bg-[#eff6ff] h-[3780px]">
    <div class="container mx-auto 2xl:pt-[22px]">
      <div class="bg-white 2xl:p-5 2xl:flex 2xl:pt[-22px] overflow-hidden 2xl:pb-[22px] 2xl:gap-[30px] pt-[22px] flex pb-[22px] gap-[28px]">
        <div class="w-[250px] ml-[14px] 2xl:w-[300px]">
          <p class="pt-[16px] h-[56px] text-[22px] hover:bg-[#E5F1FF] hover:font-bold rounded-[6px] pl-[12px]">Automobiles
          </p>
          <p class="pt-[16px] h-[56px] text-[20px] hover:bg-[#E5F1FF] hover:font-bold rounded-[6px] pl-[12px]">Clothes and
            wear</p>
          <p class="pt-[16px] h-[56px] text-[20px] hover:bg-[#E5F1FF] hover:font-bold rounded-[6px] pl-[12px]">Home
            interiors</p>
          <p class="pt-[16px] h-[56px] text-[20px] hover:bg-[#E5F1FF] hover:font-bold rounded-[6px] pl-[12px]">Computer
            and tech</p>
          <p class="pt-[16px] h-[56px] text-[20px] hover:bg-[#E5F1FF] hover:font-bold rounded-[6px] pl-[12px]">Tools,
            equipments</p>
          <p class="pt-[16px] h-[56px] text-[20px] hover:bg-[#E5F1FF] hover:font-bold rounded-[6px] pl-[12px]">Sports and
            outdoor</p>
          <p class="pt-[16px] h-[56px] text-[20px] hover:bg-[#E5F1FF] hover:font-bold rounded-[6px] pl-[12px]">Animal and
            pets</p>
          <p class="pt-[16px] h-[56px] text-[20px] hover:bg-[#E5F1FF] hover:font-bold rounded-[6px] pl-[12px]">Machinery
            tools</p>
          <p class="pt-[16px] h-[56px] text-[20px] hover:bg-[#E5F1FF] hover:font-bold rounded-[6px] pl-[12px]">More
            category</p>
        </div>

        <div class="">
          <h1 class="absolute mt-[54px] ml-[50px] text-[32px]">Latest trending</h1>
          <h1 class="absolute mt-[95px] ml-[50px] text-[38px]"><b>Electronic items</b></h1>
          <button class="absolute mt-[165px] ml-[50px] text-[20px] bg-white rounded-md p-3">Learn More</button>
          <img class="w-[910px]" src="../public/images/eItems.png" alt="">
        </div>
        <div class="flex flex-col justify-around">
          <div class="w-[280px] h-[200px] bg-[#E3F0FF] flex flex-col items-center rounded-[6px]">
            <div class="flex pt-[16px] gap-[12px] mb-[14px]">
              <img class="w-[60px]" src="../public/icons/avatar.svg" alt="">
              <p class="text-[20px]">Hi, user <br>let's get stated</p>
            </div>
            <button class="bg-[#127FFF] text-white w-[240px] h-[46px] rounded-[6px] text-[18px]">Join now</button>
            <button
              class="mt-[7px] bg-white rounded-[6px] text-[#0D6EFD] w-[240px] h-[45px] border text-[18px]">Login</button>
          </div>
          <div class="h-[130px] bg-[#F38332] rounded-md flex items-center">
            <p class="text-[20px] ml-[25px] text-white mb-3">Get US $10 off <br>with a new <br>supplier</p>
          </div>
          <div class="h-[130px] bg-[#55BDC3] rounded-md flex items-center">
            <p class="text-[20px] ml-[25px] text-white mb-3">Send quotes with <br>supplier <br>preferences</p>
          </div>
        </div>
      </div>
      <div class="bg-white mt-[30px] pl-[20px]  h-[310px] rounded-[10px] flex border border-gray-200">
        <div class="w-[300px] mt-[20px] mr-[100px]">
          <h1 class="font-bold text-[24px]">Deals and offers</h1>
          <p class="text-[#8B96A5] text-[20px]">Hygiene equipments</p>
          <div class="mt-[20px]">
            <button class="w-[55px] h-[60px] text-white bg-[#606060] rounded-[4px]">
              <h1 class="font-bold">04</h1>
              Days
            </button>
            <button class="ml-[6px] mr-[6px] w-[55px] h-[60px] text-white bg-[#606060] rounded-[4px]">
              <h1 class="font-bold">13</h1>
              Hour
            </button>
            <button class="mr-[6px] w-[55px] h-[60px] text-white bg-[#606060] rounded-[4px]">
              <p class="font-bold">34</p>
              Min
            </button>
            <button class="w-[55px] h-[60px] text-white bg-[#606060] rounded-[4px]">
              <p class="font-bold">56</p>
              Sec
            </button>
          </div>
        </div>

        <div class="flex">
          <div v-for="el in  OfferLinks" class="w-[235px] border flex flex-col items-center pt-[18px]">
            <img :src="`/images/${el.img}`" alt="" class="w-[180px] h-[180px]" />
            <span class="mt-[11px] text-[21px]">{{ el.title }}</span>
            <button class="mt-[8px] bg-[#FFE3E3] text-[#EB001B] w-[75px] h-[40px] rounded-full">
              {{ el.number }}
            </button>
          </div>
        </div>
      </div>

      <div class="bg-white h-[340px] mt-[21px] flex rounded-[11px] border border-gray-300">
        <div class="rounded-md">
          <div class="absolute mt-[21px] ml-[21px]">
            <h1 class="font-bold text-[24px]">
              Home and <br />
              outdoor
            </h1>
            <button class="w-[150px] h-[50px] text-[20px] bg-white rounded-[6px] mt-[20px]">
              Source now
            </button>
          </div>
          <img class="w-[360px] h-full" src="../public/images/flowers.png" alt="" />
        </div>
        <div class="w-[1175px] grid grid-cols-4">
          <div v-for=" el  in   HomeLinks  " class="border relative">
            <div class="mt-[20px] ml-[16px]">
              <span class="text-[22px]">{{ el.title }}</span>
              <p class="text-[#8B96A5] mt-[9px]">
                From <br />
                USD {{ el.price }}
              </p>
            </div>
            <img class="absolute bottom-0 right-0 mr-[9px] mb-[9px] w-[105px] h-[105px]" :src="`/images/${el.img}`"
              alt="" />
          </div>
        </div>
      </div>

      <div class="bg-white h-[340px] mt-[24px] flex rounded-[11px] border border-gray-300">
        <div class="">
          <div class="absolute mt-[21px] ml-[21px]">
            <h1 class="font-bold text-[24px]">
              Consumer <br />
              electronics and <br />
              gadgets
            </h1>
            <button class="w-[150px] h-[50px] text-[20px] bg-white rounded-[6px] mt-[20px]">
              Source now
            </button>
          </div>
          <img class="w-[360px] h-full" src="../public/images/gadgets.png" alt="" />
        </div>
        <div class="w-[1175px] grid grid-cols-4">
          <div v-for="  el   in   ElectronicLinks  " class="border relative">
            <div class="mt-[21px] ml-[16px]">
              <span class="text-[23px]">{{ el.title }}</span>
              <p class="text-[#8B96A5] mt-[10px]">
                From <br />
                USD {{ el.price }}
              </p>
            </div>
            <img class="absolute bottom-0 right-0 mr-[9px] mb-[9px] w-[100px] h-[100px]" :src="`/images/${el.img}`"
              alt="" />
          </div>
        </div>
      </div>

      <div class="bg-white mt-[20px]">
        <div class="absolute text-white mt-[50px] ml-[50px]">
          <h1 class="text-[40px] font-bold">
            An easy way to send <br />
            requests to all suppliers
          </h1>
          <p class="text-[20px] mt-[18px]">
            Lorem ipsum dolor sit amet, consectetur adipisicing <br />
            elit, sed do eiusmod tempor incididunt.
          </p>
        </div>
        <div class="absolute ml-[850px] w-[630px] mt-[50px] h-[450px] rounded-[6px] bg-white pt-[30px] pl-[40px]">
          <h1 class="text-[24px] font-bold">Send quote to suppliers</h1>
          <input
            class="placeholder-black rounded-[6px] w-[530px] border h-[50px] flex items-center text-[21px] mt-[21px] pl-[15px]"
            type="text" placeholder="What item you need?">
          <textarea
            class="mt-[25px] border border-gray-200 rounded-md w-[530px] py-2 px-3 placeholder-gray-300 text-[21px] leading-tight outline-none"
            name="details" id="details" cols="30" rows="3" placeholder="Type more details"></textarea>
          <div class="flex">
            <input
              class="placeholder-black rounded-[6px] mt-[25px] border text-[21px] w-[250px] pl-[12px] flex items-center h-[50px]"
              type="text" name="" id="" placeholder="Quantity">
            <select
              class="rounded-md h-[50px] mt-[25px] ml-[15px] w-[130px] py-2 px-3 text-black text-[21px] leading-tight focus:outline-none"
              name="select" id="select">
              <option value="1">Pcs</option>
              <option value="2">Junior</option>
              <option value="3">Middle</option>
              <option value="2">Senior</option>
            </select>
          </div>

          <button class="bg-[#127FFF] text-white w-[170px] text-[20px] h-[50px] mt-[30px] rounded-[6px]">
            Send inquiry
          </button>
        </div>
        <img class="rounded-[6px] w-full" src="../public/images/bgImage.png" alt="" />
      </div>
      <div class="mt-[25px]">
        <h1 class="text-[28px] font-bold">Recommended items</h1>
        <div class="grid grid-cols-5 gap-[31px] mt-[31px]">
          <div v-for="el in RecItemsLinks" class="rounded-[8px] border bg-white h-[410px]">
            <div class="flex flex-col items-center mt-[26px]">
              <img class="w-[240px] h-[240px]" :src="`/images/${el.img}`" alt="" />
            </div>
            <h1 class="ml-[16px] text-[22px] mt-[30px]">{{ el.price }}</h1>
            <p class="ml-[16px] text-[18px] text-[#8B96A5] mt-[5px] w-[180px]">
              {{ el.desc }}
            </p>
          </div>
        </div>
      </div>

      <div class="mt-[30px]">
        <h1 class="text-[28px] font-semibold">Our extra services</h1>
        <div class="grid grid-cols-4 gap-[25px]">
          <div class="w-[362px] h-[270px] bg-white mt-[24px] rounded-[8px]">
            <img class="w-full bg-[#374151] h-[160px] rounded-t-[6px]" src="../public/images/service1.png" alt="" />
            <p class="text-[20px] mt-[25px] ml-[30px] font-medium">
              Source from<br />Industry Hubs
            </p>

            <div
              class="border-white border-[3px] mt-[-120px] ml-[250px] absolute bg-[#D1E7FF] w-[80px] h-[80px] rounded-full flex justify-center items-center">
              <img class="w-[25px] h-[25px]" src="../public/icons/lupa.svg" alt="" />
            </div>
          </div>

          <div class="w-[362px] h-[270px] bg-white mt-[24px] rounded-[8px]">
            <img class="bg-[#374151] h-[160px] rounded-t-[6px]" src="../public/images/service2.png" alt="" />
            <p class="text-[20px] mt-[25px] ml-[30px] font-medium">
              Customize Your <br /> Products
            </p>

            <div
              class="border-white border-[3px] mt-[-120px] ml-[250px] absolute bg-[#D1E7FF] w-[80px] h-[80px] rounded-full flex justify-center items-center">
              <img class="w-[25px] h-[25px]" src="../public/icons/box.svg" alt="" />
            </div>
          </div>


          <div class="w-[362px] h-[270px] bg-white mt-[24px] rounded-[8px]">
            <img class="bg-[#374151] h-[160px] rounded-t-[6px]" src="../public/images/service3.png" alt="" />
            <p class="text-[20px] mt-[25px] ml-[30px] font-medium">
              Fast, reliable shipping<br />by ocean or air
            </p>

            <div
              class="border-white border-[3px] mt-[-120px] ml-[250px] absolute bg-[#D1E7FF] w-[80px] h-[80px] rounded-full flex justify-center items-center">
              <img class="w-[25px] h-[25px]" src="../public/icons/plane.svg" alt="" />
            </div>
          </div>

          <div class="w-[362px] h-[270px] bg-white mt-[24px] rounded-[8px]">
            <img class="bg-[#374151] h-[160px] rounded-t-[6px]" src="../public/images/service4.png" alt="" />
            <p class="text-[20px] mt-[25px] ml-[30px] font-medium">
              Product monitoring<br />and Inspection
            </p>

            <div
              class="border-white border-[3px] mt-[-120px] ml-[250px] absolute bg-[#D1E7FF] w-[80px] h-[80px] rounded-full flex justify-center items-center">
              <img class="w-[25px] h-[25px]" src="../public/icons/defend.svg" alt="" />
            </div>
          </div>
        </div>
      </div>


      <div class="mt-[31px]">
        <h1 class="text-[28px] font-semibold">Suppliers by region</h1>
        <div>
          <div class="grid grid-cols-5 mt-[10px]">
            <div class="flex mt-[16px] items-center" v-for="el in RepublicLinks">
              <img class="w-[40px] h-[30px]" :src="`/images/${el.img}`" alt="" />
              <div class="ml-[15px]">
                <h1 class="text-[20px]">{{ el.title }}</h1>
                <p class="text-[#8B96A5] text-[16px]">{{ el.desc }}</p>
              </div>
            </div>
          </div>

          <div></div>
        </div>
      </div>
    </div>

  </main>

  <Footer2 />
</template>

<script setup>
const OfferLinks = [
  {
    id: 1,
    title: "Smart watches",
    img: "smartWatches.png",
    number: "-25%",
  },
  {
    id: 2,
    title: "Laptops",
    img: "laptop.png",
    number: "-15%",
  },
  {
    id: 3,
    title: "GoPro cameras",
    img: "goProCamera.png",
    number: "-40%",
  },
  {
    id: 4,
    title: "Headphones",
    img: "headphones.png",
    number: "-25%",
  },
  {
    id: 5,
    title: "Canon camreras",
    img: "canonCamera.png",
    number: "-25%",
  },
];

const HomeLinks = [
  {
    id: 1,
    title: "Soft chairs",
    price: 19,
    img: "chair.png",
  },
  {
    id: 2,
    title: "Sofa & chair",
    price: 19,
    img: "sofaChair.png",
  },
  {
    id: 3,
    title: "Kitchen dishes",
    price: 19,
    img: "dishes.png",
  },
  {
    id: 4,
    title: "Smart watches",
    price: 19,
    img: "qozon.png",
  },
  {
    id: 5,
    title: "Kitchen mixer",
    price: 100,
    img: "mixer.png",
  },
  {
    id: 6,
    title: "Blenders",
    price: 39,
    img: "blender.png",
  },
  {
    id: 7,
    title: "Home appliance",
    price: 19,
    img: "homeAppliance.png",
  },
  {
    id: 8,
    title: "Coffee maker",
    price: 10,
    img: "flower.png",
  },
];

const ElectronicLinks = [
  {
    id: 1,
    title: "Smart watches",
    price: 19,
    img: "smartWatches.png",
  },
  {
    id: 2,
    title: "Cameras",
    price: 89,
    img: "goProCamera.png",
  },
  {
    id: 3,
    title: "Headphones",
    price: 10,
    img: "headphone2.png",
  },
  {
    id: 4,
    title: "Smart watches",
    price: 90,
    img: "tefal.png",
  },
  {
    id: 5,
    title: "Gaming set",
    price: 35,
    img: "headphones.png",
  },
  {
    id: 6,
    title: "Laptops & PC",
    price: 340,
    img: "laptop.png",
  },
  {
    id: 7,
    title: "Smartphones",
    price: 19,
    img: "planshet.png",
  },
  {
    id: 8,
    title: "Electric kattle",
    price: 240,
    img: "iphone.png",
  },
];

const RecItemsLinks = [
  {
    id: 1,
    price: "$10.30",
    desc: "T-shirts with multiple colors, for men",
    img: "recItem1.png",
  },
  {
    id: 2,
    price: "$10.30",
    desc: "Jeans shorts for men blue color",
    img: "recItem2.png",
  },
  {
    id: 3,
    price: "$12.50",
    desc: "Brown winter coat medium size",
    img: "recItem3.png",
  },
  {
    id: 4,
    price: "$34.00",
    desc: "Jeans bag for travel for men",
    img: "recItem4.png",
  },
  {
    id: 5,
    price: "$99.00",
    desc: "Leather wallet",
    img: "recItem5.png",
  },
  {
    id: 6,
    price: "$9.99",
    desc: "Canon camera black, 100x zoom",
    img: "recItem6.png",
  },
  {
    id: 7,
    price: "$8.99",
    desc: "Headset for gaming with mic",
    img: "headphone2.png",
  },
  {
    id: 8,
    price: "$10.30",
    desc: "Smartwatch silver color modern",
    img: "popka.png",
  },
  {
    id: 9,
    price: "$10.30",
    desc: "Blue wallet for men leather metarfial",
    img: "qozon.png",
  },
  
  {
    id: 10,
    price: "$80.95",
    desc: "Jeans bag for travel for men",
    img: "recItem10.png",
  },
];


const RepublicLinks = [
  {
    id: 1,
    img: "uae.png",
    title: "Arabic Emirates",
    desc: "shopname.ae"
  },

  {
    id: 2,
    img: "australia.png",
    title: "Australia",
    desc: "shopname.ae"
  },

  {
    id: 3,
    img: "us.png",
    title: "United States",
    desc: "shopname.ae"
  },

  {
    id: 4,
    img: "russia.png",
    title: "Russia",
    desc: "shopname.ru"
  },

  {
    id: 5,
    img: "italy.png",
    title: "Italy",
    desc: "shopname.it"
  },

  {
    id: 6,
    img: "denmark.png",
    title: "Denmark",
    desc: "denmark.com.dk"
  },

  {
    id: 7,
    img: "france.png",
    title: "France",
    desc: "shopname.com.fr"
  },

  {
    id: 8,
    img: "uae.png",
    title: "Arabic Emirates",
    desc: "shopname.ae"
  },

  {
    id: 9,
    img: "china.png",
    title: "China",
    desc: "shopname.ae"
  },

  {
    id: 10,
    img: "uk.png",
    title: "Great Britain",
    desc: "shopname.co.uk"
  },

]
</script>

<style lang="scss" scoped></style>