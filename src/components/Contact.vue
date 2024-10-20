<script setup> </script>
<template>
    <div class="bg-[#0E1F51] py-10">
      <div class="text-center mt-8">
      <h2 class="text-2xl font-semibold mb-6 text-[#FF3E54] text-[24px]">\ Get In Touch \</h2>
      <p class="text-3xl font-bold mb-16 text-[42px] text-white">Hey! Let's Talk</p>
    </div>
      <div class=" max-w-7xl left-1 mx-auto grid place-items-center grid-cols-1 md:grid-cols-2 ">
        <!-- Left Form Section -->
        <div class="bg-white p-8 rounded-lg shadow-md w-full w-96 h-full ">
          <!-- Form -->
          <form @submit.prevent="submitForm">
            <!-- Name -->
            <div class="mb-4">
              <input
                type="text"
                v-model="form.name"
                placeholder="Name"
                class="w-full px-4 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-indigo-500"
                required
              />
            </div>
  
            <!-- Email -->
            <div class="mb-4">
              <input
                type="email"
                v-model="form.email"
                placeholder="Email"
                class="w-full px-4 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-indigo-500"
                required
              />
            </div>
  
            <!-- Phone -->
            <div class="mb-4">
              <input
                type="text"
                v-model="form.phone"
                placeholder="Phone"
                class="w-full px-4 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-indigo-500"
                required
              />
            </div>
  
            <!-- Message -->
            <div class="mb-4">
              <textarea
                v-model="form.message"
                placeholder="Your Message"
                class="w-full px-4 py-2 border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-indigo-500"
                rows="4"
                required
              ></textarea>
            </div>
  
            <!-- Submit Button -->
            <button
              type="submit"
              class="w-full py-2 px-4 bg-red-500 text-white font-semibold rounded-md hover:bg-red-600 transition duration-200"
            >
              Send Now
            </button>
          </form>
        </div>
  
        <!-- Right Contact Info Section -->
        <div class="bg-white p-8 rounded-lg shadow-md w-full md:w-96 h-full">
          <div class="mb-6">
            <h3 class="text-xl font-semibold text-indigo-900">Call Anytime</h3>
            <p class="text-gray-600">+91 23678 27867<br />+91 67678 92878</p>
          </div>
  
          <div class="mb-6">
            <h3 class="text-xl font-semibold text-indigo-900">Send Email</h3>
            <p class="text-gray-600">connect@itfirms.com<br />hello@itfirms.com</p>
          </div>
  
          <div class="mb-6">
            <h3 class="text-xl font-semibold text-indigo-900">Visit Us</h3>
            <p class="text-gray-600">20 Island Park Road, New Jersey, New York, USA</p>
          </div>
  
          <h3 class="text-xl font-semibold text-indigo-900">Follow us</h3>
          <div class="flex space-x-4 mt-4">
            <a href="#" class="text-red-500"><i class="fab fa-linkedin"></i></a>
            <a href="#" class="text-red-500"><i class="fab fa-instagram"></i></a>
            <a href="#" class="text-red-500"><i class="fab fa-facebook"></i></a>
            <a href="#" class="text-red-500"><i class="fab fa-twitter"></i></a>
          </div>
        </div>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        form: {
          name: '',
          email: '',
          phone: '',
          message: ''
        }
      };
    },
    methods: {
      submitForm() {
        const { name, email, phone, message } = this.form;
  
        // For demonstration purposes, we'll log the form data to the console
        console.log('Form Data:', { name, email, phone, message });
  
        // Reset form after submission
        this.form.name = '';
        this.form.email = '';
        this.form.phone = '';
        this.form.message = '';
  
        alert('Message Sent Successfully!');
      }
    }
  };
  </script>
  <script setup>
  import { Facebook } from 'lucide-vue-next';
  </script>
  
  
  <style scoped>
  /* Additional styles, if any */
  </style>
  