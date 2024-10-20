<script setup></script>
<template>
    <div class="py-10 bg-gray-100">
      <div class="text-center mb-8">
        <h2 class="text-[#FF3E54] text-[24px] font-bold">\ Our Blog \</h2>
        <p class=" font-bold text-[40px] text-black">Latest Post</p>
      </div>
      <div class="flex justify-center gap-6">
        <div v-for="(post, index) in posts" :key="index" class="bg-white rounded-lg shadow-md p-4 w-80">
          <img :src="post.image" alt="Post image" class="rounded-t-lg object-cover h-48 w-full">
          <h3 class="text-lg font-semibold text-red-600 mt-4">{{ post.title }}</h3>
          <div class="flex items-center mt-2">
            <img :src="post.authorImage" alt="Author image" class="w-8 h-8 rounded-full mr-2">
            <div>
              <p class="text-sm font-medium">{{ post.author }}</p>
              <p class="text-xs text-gray-500">{{ post.date }}</p>
            </div>
          </div>
        </div>
      </div>
    </div>
    
  </template>
  
  <script>
  export default {
    data() {
      return {
        posts: [
          {
            title: 'The most Popular Business Of the Year',
            author: 'Ranold Jeff.',
            date: 'May 4th, 2022',
            image: 'src/assets/icons/images/dca3abcfff8774f613f072049cc8cd33.jpg',
            authorImage: 'src/assets/icons/images/2ffb7c3f3f27c0a9aa612e7902b7797b.jpg'
          },
          {
            title: 'The most Popular Business Of the Year',
            author: 'Patricia Anderson',
            date: 'Apr 27th, 2022',
            image: 'src/assets/icons/images/1d7329846faf5774501ca998db2edb6b.jpg',
            authorImage: 'src/assets/icons/images/e41d77f1377f41b9a561e50ab2257382.jpg'
          },
          {
            title: 'The most Popular Business Of the Year',
            author: 'Elaine Luna',
            date: 'Apr 20th, 2022',
            image: 'src/assets/icons/images/3d161a1ec4f5ce64bcdcdf4e6d6dc75c.jpg',
            authorImage: 'src/assets/icons/images/81ad50acaef58c1a9981df8cf937dd37.jpg'
          }
        ]
      }
    }
  }
  </script>
  
  <style scoped>
  /* Custom styles for the component */
  </style>
  