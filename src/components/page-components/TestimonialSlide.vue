<script>
    export default {
    data() {
        return {
        currentSlide: 0,
        testimonials: [
            {
            name: 'Samual Karl',
            position: 'CEO',
            text: 'It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout. The point of using Lorem Ipsum is that it has a more-or-less normal distribution of letters, as opposed.',
            image: 'https://randomuser.me/api/portraits/men/32.jpg'
            },
            {
            name: 'Daria Linney',
            position: 'CEO',
            text: 'It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout. The point of using Lorem Ipsum is that it has a more-or-less normal distribution of letters, as opposed.',
            image: 'https://randomuser.me/api/portraits/women/44.jpg'
            },
            {
            name: 'Daria Linney',
            position: 'CEO',
            text: 'It is a long established fact that a reader will be distracted by the readable content of a page when looking at its layout. The point of using Lorem Ipsum is that it has a more-or-less normal distribution of letters, as opposed.',
            image: 'https://randomuser.me/api/portraits/women/44.jpg'
            },
        ]
        };
    },
    methods: {
        nextSlide() {
        this.currentSlide = (this.currentSlide + 1) % this.testimonials.length;
        },
        prevSlide() {
        this.currentSlide = (this.currentSlide - 1 + this.testimonials.length) % this.testimonials.length;
        },
        setSlide(index) {
        this.currentSlide = index;
        }
    }
    };
</script>


<template>
    <div class="flex flex-col items-center py-10">

      <!-- Slider Section -->
      <div class="relative mt-8 w-full max-w-4xl">
        <div class="flex justify-between items-center">
          <button @click="prevSlide" class="text-3xl font-bold text-gray-400 hover:text-gray-600 hidden">
            &#60;
          </button>
  
          <div class="flex items-center w-full mx-4 overflow-hidden">
            <transition-group name="slide" tag="div" class="flex space-x-6">
              <div v-for="(testimonial, index) in testimonials" :key="index" v-show="currentSlide === index" class="flex-none w-full p-6 bg-[#F7F7F7] rounded-md">
                <div>
                  <div class="flex justify-between">
                    <img :src="testimonial.image" class="w-[75px] h-[75px] rounded-full mb-4" alt="User Image">
                    <img src="/src/assets/quote-marks.png" class="h-[40px]">
                  </div>
                  <p class="text-[#252525] text-[16px] my-7 mr-[150px]">{{ testimonial.text }}</p>
                  <p class="text-[16px] font-bold text-[#FF3E54]">{{ testimonial.name }}</p>
                  <p class="text-[14px] text-[#0E1F51] font-medium">{{ testimonial.position }}</p>
                </div>
              </div>
            </transition-group>
          </div>
  
          <button @click="nextSlide" class="text-3xl font-bold text-gray-400 hover:text-gray-600 hidden">
            &#62;
          </button>
        </div>
  
        <!-- Dots Navigation -->
        <div class="flex justify-center space-x-2 mt-4">
          <span v-for="(testimonial, index) in testimonials" :key="index" @click="setSlide(index)"
                :class="['w-4 h-4 rounded-full cursor-pointer', currentSlide === index ? 'bg-[#FF3E54]' : 'border-[1px] border-[#FF3E54]']">
          </span>
        </div>
      </div>
    </div>
</template>
  
  
<style scoped>
    /* Custom animation for slide transition */
    .slide-enter-active, .slide-leave-active {
    transition: all 0.5s;
    }
    .slide-enter, .slide-leave-to {
    transform: translateX(100%);
    opacity: 0;
    }
</style>
  