<script setup></script>
<template>
    <div>
      <!-- About Us Hero Section -->
      <section class="bg-blue-900 text-white py-10">
        <div class="container mx-auto text-center">
          <h2 class="text-4xl font-bold mb-2">About</h2>
          <p>Home / About</p>
        </div>
      </section>
  
      <!-- Content Section -->
      <section class="bg-gray-100 py-16">
        <div class="container mx-auto grid grid-cols-2 gap-8 items-center">
          <!-- Image Section -->
          <div>
            <img src="/src/assets/Mask group.svg" alt="People working together" class="rounded-lg shadow-lg">
          </div>
          
          <!-- Text Section -->
          <div>
            <h3 class="text-red-500 font-bold text-lg mb-2">\ About us \</h3>
            <h1 class="text-4xl font-bold text-gray-900 mb-4">One of the Fastest Ways to Business Growth</h1>
            <p class="text-lg text-gray-600 mb-6">
              It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout. The point of using Lorem Ipsum is that it has a more-or-less normal distribution of letters...
            </p>
            
            <!-- CTA Box -->
            <div class="bg-white p-6 rounded-lg shadow-md flex items-center space-x-4">
              <div class="bg-red-100 p-4 rounded-full">
              </div>
              <div>
                <p class="text-gray-900 font-bold">Get Instant Professional Advice</p>
                <p class="text-red-500 font-semibold">Ready to Help: +1 356 678 7897</p>
              </div>
            </div>
          </div>
        </div>
      </section>
    </div>
    <section class="py-16">
      <div class="container mx-auto text-center">
        <h2 class="text-4xl font-bold mb-12">Our Leaders</h2>
        <div class="grid grid-cols-4 gap-8">
          <div v-for="leader in leaders" :key="leader.name" class="text-center">
            <img :src="leader.image" alt="leader.name" class="rounded-full mx-auto mb-4" width="150" height="150" />
            <h3 class="text-2xl font-bold">{{ leader.name }}</h3>
            <p class="text-lg text-gray-600">{{ leader.role }}</p>
          </div>
        </div>
      </div>
    </section>
    <section>
        <div>
    <!-- Banner Section -->
    <section class="py-12 text-center">
      <div class="max-w-xl mx-auto bg-blue-900 text-white p-8 rounded-md shadow-lg">
        <p class="text-lg font-semibold">"Some of the History of Our Company is that we are Catching up through Video"</p>
        <button class="mt-4 bg-red-500 text-white px-4 py-2 rounded">Get In Touch</button>
      </div>
    </section>

    <!-- Footer Section -->
    <footer class="bg-blue-900 text-white py-8">
      <div class="max-w-5xl mx-auto grid grid-cols-4 gap-8 text-center">
        <!-- About Us -->
        <div>
          <h3 class="text-xl font-semibold mb-4">About Us</h3>
          <p class="text-sm">
            It is a long established fact that a reader will be distracted by the readable content of a page.
          </p>
        </div>
        
        <!-- Services -->
        <div>
          <h3 class="text-xl font-semibold mb-4">Services</h3>
          <ul class="text-sm">
            <li>Web Design/Development</li>
            <li>App Development</li>
          </ul>
        </div>
        
        <!-- Career -->
        <div>
          <h3 class="text-xl font-semibold mb-4">Career</h3>
          <div class="text-sm">
            <p class="font-bold">ReactJS Dev.</p>
            <p>1-5 Years of Exp.</p>
          </div>
        </div>

        <!-- Subscribe Us -->
        <div>
          <h3 class="text-xl font-semibold mb-4">Subscribe Us</h3>
          <p class="text-sm">
            It is a long established fact that a reader will be distracted by the readable content of a page.
          </p>
        </div>
      </div>
    </footer>
  </div>    
    </section>
  </template>
  

  

  

  <script>
export default {
  data() {
    return {
      leaders: [
        { name: 'Larry P. Burnett', role: 'CEO', image: 'src/assets/Rectangle 14.svg' },
        { name: 'Meghan J. Weiss', role: 'CTO', image: 'src/assets/Rectangle 15.svg' },
        { name: 'Yvonne J. Dufour', role: 'CFO', image: 'src/assets/Rectangle 16.svg' },
        { name: 'Diana K. Williams', role: 'COO', image: 'src/assets/Rectangle 17 (1).svg' },
        { name: 'Larry P. Burnett', role: 'CEO', image: 'src/assets/Rectangle 14.svg' },
        { name: 'Meghan J. Weiss', role: 'CTO', image: 'src/assets/Rectangle 15.svg' },
        { name: 'Yvonne J. Dufour', role: 'CFO', image: 'src/assets/Rectangle 16.svg' },
        { name: 'Diana K. Williams', role: 'COO', image: 'src/assets/Rectangle 17 (1).svg' }

      ]
    }
  }
}
</script>
  <style scoped>
  .container {
    max-width: 1200px;
    padding-left: 20px;
    padding-right: 20px;
  }
  </style>
  