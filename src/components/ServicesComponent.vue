<script setup>
import { faCode, faMobileAlt, faCloud, faRobot, faBullhorn } from '@fortawesome/free-solid-svg-icons'

const services = [
  { 
    name: "Web Development", 
    icon: faCode,
    description: "Custom websites and web applications tailored to your needs"
  },
  { 
    name: "Mobile Apps", 
    icon: faMobileAlt,
    description: "Native and cross-platform mobile solutions"
  },
  { 
    name: "Cloud Services", 
    icon: faCloud,
    description: "Scalable cloud infrastructure and deployment"
  },
  { 
    name: "AI Solutions", 
    icon: faRobot,
    description: "Intelligent automation and machine learning"
  },
  { 
    name: "Digital Marketing", 
    icon: faBullhorn,
    description: "SEO, social media, and comprehensive digital marketing strategies"
  }
]
</script>

<template>
  <section class="bg-gradient-to-b from-blue-500 to-blue-600 py-16 px-4">
    <div class="max-w-6xl mx-auto text-center mb-12">
      <h1 class="text-white text-4xl md:text-5xl font-bold mb-4">
        Our Services
      </h1>
      <p class="text-blue-100 text-lg md:text-xl max-w-2xl mx-auto">
        We provide comprehensive solutions across all technology domains
      </p>
    </div>
   
    <!-- Services Grid -->
    <div class="max-w-6xl mx-auto grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-6">
      <div 
        v-for="service in services" 
        :key="service.name" 
        class="bg-white rounded-xl shadow-lg p-8 text-center transition-all duration-300 hover:shadow-2xl hover:-translate-y-2 hover:bg-blue-50 cursor-pointer group"
      >
        <!-- Icon -->
        <div class="mb-6 transition-transform duration-300 group-hover:scale-110">
          <font-awesome-icon 
            :icon="service.icon" 
            class="text-blue-500 group-hover:text-blue-600" 
            size="3x" 
          />
        </div>
        
        <!-- Title -->
        <h2 class="text-xl font-bold text-gray-800 mb-3">
          {{ service.name }}
        </h2>
        
        <!-- Description -->
        <p class="text-gray-600 text-sm leading-relaxed">
          {{ service.description }}
        </p>
      </div>
    </div>
  </section>
</template>