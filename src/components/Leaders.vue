<template>
    <div class="team-container py-10">
      <!-- Section Title -->
      <div class="grid grid-cols-1 text-center font-bold">
            <p class="text-[#FF3E54] text-[24px]">\ Team \</p>
            <h1 class="text-[#0E1F51] text-[40px]">Our Leaders</h1>
        </div>
  
      <!-- Leaders Grid -->
      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 mt-16 gap-16 max-w-6xl mx-auto">
        <div v-for="member in leaders" :key="member.id" class="team-member text-center">
          <!-- Image -->
          <img
            :src="member.image"
            alt="Team member photo"
            class="w-80 h-80 mx-auto rounded-lg mb-4 object-cover"
          />
          <!-- Name -->
          <h3 class="text-xl font-semibold text-gray-800">{{ member.name }}</h3>
          <!-- Role -->
          <p class="text-indigo-600 text-md">{{ member.role }}</p>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        leaders: [
          {
            id: 1,
            name: 'Larry F. Burnett',
            role: 'CEO',
            image: 'src/assets/icons/images/image.png'
          },
          {
            id: 2,
            name: 'Meghan J. Webb',
            role: 'CEO',
            image: 'src/assets/icons/images/image.png'
          },
          {
            id: 3,
            name: 'Yvonne J. Cullum',
            role: 'CEO',
            image: 'src/assets/icons/images/image.png'
          },
          {
            id: 4,
            name: 'Diana H. Williams',
            role: 'CEO',
            image: 'src/assets/icons/images/image.png'
          }
        ]
      };
    }
  };
  </script>
  
  <style scoped>
  /* Optional additional styling */
  .team-container {
    background-color: #f9fafb;
  }
  
  .team-member img {
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  }
  </style>
  