<script setup>
import team3 from "@/assets/team3.jpeg" 
</script>

<template>
  <section class="bg-gradient-to-br from-gray-50 to-gray-100 py-16 px-4">
    <!-- Header -->
    <div class="max-w-6xl mx-auto text-center mb-12">
      <h1 class="text-4xl md:text-5xl font-bold text-gray-800 mb-4">
        Who We Are
      </h1>
      <p class="text-gray-600 text-lg md:text-xl">
        Innovating Tomorrow's Digital Landscape
      </p>
    </div>

    <!-- Content Container -->
    <div class="max-w-6xl mx-auto flex flex-col md:flex-row items-center gap-8 md:gap-12">
      <!-- Image -->
      <div class="w-full md:w-1/2 flex justify-center">
        <img 
          :src="team3" 
          alt="KLUMUS Technologies Team" 
          class="w-full max-w-md h-auto rounded-2xl shadow-2xl object-cover transition-transform duration-300 hover:scale-105"
        />
      </div>

      <!-- Text Content -->
      <div class="w-full md:w-1/2">
        <p class="text-gray-700 text-lg leading-relaxed">
          At <span class="font-bold text-blue-600">KLUMUS Technologies</span>, we are a team of innovators transforming ideas into advanced digital solutions. We deliver high-quality, customer-focused services across web development, mobile apps, cloud computing, and AI technologies—combining creativity and technology to build functional, user-centered, and impactful solutions.
        </p>
        
        <!-- Optional: Add a CTA button -->
        <div class="mt-8">
          <a 
            href="#" 
            class="inline-block bg-blue-600 text-white font-semibold px-8 py-3 rounded-lg shadow-lg hover:bg-blue-700 hover:shadow-xl transition-all duration-300 hover:-translate-y-1"
          >
            Learn More About Us
          </a>
        </div>
      </div>
    </div>
  </section>
</template>