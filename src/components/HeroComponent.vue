<script setup>
import bgImage from "@/assets/bg1.jpeg" 

// Compute inline style for the background
const heroStyle = {
  backgroundImage: `linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url(${bgImage})`,
  backgroundSize: "cover",
  backgroundPosition: "center",
  backgroundAttachment: "fixed",
  minHeight: "70vh"
}
</script>

<template>
  <section :style="heroStyle" class="flex flex-col justify-center items-center px-4 py-20">
    <!-- Overlay Content Container -->
    <div class="max-w-4xl text-center space-y-6">
      <!-- Main Heading -->
      <h1 class="text-white text-4xl md:text-6xl font-bold drop-shadow-lg animate-fade-in">
        KLUMUS Technologies
      </h1>
      
      <!-- Tagline -->
      <p class="text-white text-xl md:text-2xl font-light drop-shadow-md">
        Innovating Tomorrow's Digital Landscape
      </p>
      
      <!-- Description -->
      <p class="text-white text-base md:text-lg max-w-2xl mx-auto drop-shadow-md opacity-90">
        Transforming ideas into cutting-edge digital solutions with expertise in web development, mobile apps, cloud services, and AI technologies.
      </p>

      <!-- Call-to-Action Buttons -->
      <div class="flex flex-wrap justify-center gap-4 mt-8">
        <a 
          href="#services" 
          class="bg-gradient-to-r from-blue-500 to-blue-700 text-white px-8 py-3 rounded-lg font-semibold shadow-lg hover:from-blue-600 hover:to-blue-800 hover:shadow-xl hover:-translate-y-1 transition-all duration-300 transform"
        >
          Explore Our Services
        </a>

        <a 
          href="#contact" 
          class="bg-white text-blue-700 px-8 py-3 rounded-lg font-semibold shadow-lg hover:bg-gray-50 hover:shadow-xl hover:-translate-y-1 transition-all duration-300 transform border-2 border-white"
        >
          Get In Touch
        </a>
      </div>
    </div>

    <!-- Scroll Indicator (Optional) -->
    <div class="absolute bottom-8 animate-bounce">
      <svg class="w-6 h-6 text-white" fill="none" stroke="currentColor" viewBox="0 0 24 24">
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 14l-7 7m0 0l-7-7m7 7V3"></path>
      </svg>
    </div>
  </section>
</template>

<style scoped>
@keyframes fade-in {
  from {
    opacity: 0;
    transform: translateY(-20px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.animate-fade-in {
  animation: fade-in 1s ease-out;
}
</style>