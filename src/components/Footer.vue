<script setup>
import { Facebook, Instagram, Linkedin, Twitter } from 'lucide-vue-next';

  
</script>

<template>
    <footer class="bg-[#0E1F51] py-10 text-white">
      <div class="container mx-auto grid grid-cols-1 md:grid-cols-4 gap-8 px-6">
        <!-- Logo Section -->
        <div>
          <div class="">
            <img src="/src/assets/Logo.png" alt="">
          </div>
          <p class="mt-4 text-[16px]">
            It is a long established fact that a reader will be distracted by the readable content of a page when looking at
          </p>
          <!-- Social Icons -->
          <div class="flex space-x-4 mt-6">
            <a href="/" class="p-2 bg-white rounded-lg text-[#FF3E54]"> <Linkedin /> </a>
            <a href="/" class="p-2 bg-white rounded-lg text-[#FF3E54]"> <Instagram /> </a>
            <a href="/" class="p-2 bg-white rounded-lg text-[#FF3E54]"> <Facebook /> </a>
            <a href="/" class="p-2 bg-white rounded-lg text-[#FF3E54]"> <Twitter /> </a>
          </div>
        </div>
  
        <!-- Services Section -->
        <div>
          <h3 class="text-[24px] font-bold mb-4">Services</h3>
          <hr class="border-[2px] rounded-full border-[#FF3E54] w-[100px] mb-4">
          <ul class="grid grid-cols-1 gap-2 text-gray-300">
            <a href="/">Web Design/Development</a>
            <a href="/">App Development</a>
            <a href="/">UI/UX Design</a>
            <a href="/">HubSpot Integration</a>
            <a href="/">Email Marketing</a>
            <a href="/">Website Migration</a>
          </ul>
        </div>
  
        <!-- Career Section -->
        <div>
          <h3 class="text-[24px] font-bold mb-4">Career</h3>
          <hr class="border-[2px] rounded-full border-[#FF3E54] w-[100px] mb-4">
          <ul class="space-y-4">
            <li class="flex items-center space-x-2">
              <div class="bg-white p-3 rounded-lg">
                <img src="/src/assets/career-icons/React.png" class="w-6 h-6 text-[#FF3E54]" />
              </div>

              <div>
                <p class="text-[#FF3E54] font-semibold">ReactJs Dev.</p>
                <p class="text-gray-300 text-sm">1-5 Years of Exp.</p>
              </div>
            </li>
            <li class="flex items-center space-x-2">
                <div class="bg-white p-3 rounded-lg">
                    <img src="/src/assets/career-icons/Wordpress.png" class="w-6 h-6 text-[#FF3E54]" />
                </div>

                <div>
                    <p class="text-[#FF3E54] font-semibold">Wordpress Dev.</p>
                    <p class="text-gray-300 text-sm">1-5 Years of Exp.</p>
                </div>
            </li>
            <li class="flex items-center space-x-2">
                <div class="bg-white p-3 rounded-lg">
                    <img src="/src/assets/career-icons/Wix.png" class="w-6 h-6 text-[#FF3E54]" />
                </div>

                <div>
                    <p class="text-[#FF3E54] font-semibold">Python Developer</p>
                    <p class="text-gray-300 text-sm">1-5 Years of Exp.</p>
                </div>
            </li>
          </ul>
        </div>
  
        <!-- Subscribe Section -->
        <div>
          <h3 class="text-lg font-semibold mb-4">Subscribe Us</h3>
          <p class="text-gray-400 text-sm mb-4">
            It is a long established fact that a reader will be distracted by the readable content
          </p>
          <div class="flex space-x-2">
            <input type="email" placeholder="Email" class="px-4 py-2 rounded-md text-black w-full" />
            <button class="bg-[#FF3E54] hover:bg-[#f13a4f] duration-100 text-white px-4 py-2 rounded-md">Submit</button>
          </div>
        </div>
      </div>
    </footer>
</template>

  
<style scoped>
    .container {
    max-width: 1200px;
    }
</style>
  