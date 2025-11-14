<script setup>
import { ref, onMounted } from 'vue'
import logo_cropped from '@/assets/logo_cropped.png'

const isToggle = ref(false)
const activeSection = ref('home')

// Smooth scroll to section without updating URL hash
const scrollToSection = (id) => {
  const el = document.getElementById(id)
  if (el) {
    const headerOffset = 80 // Adjust based on navbar height
    const elementPosition = el.getBoundingClientRect().top + window.scrollY
    const offsetPosition = elementPosition - headerOffset

    window.scrollTo({
      top: offsetPosition,
      behavior: 'smooth'
    })
  }
  isToggle.value = false // Close mobile menu after selection
}

// Observe sections to update active nav link
onMounted(() => {
  const sections = document.querySelectorAll('section[id]')
  const observer = new IntersectionObserver(
    (entries) => {
      entries.forEach((entry) => {
        if (entry.isIntersecting) {
          activeSection.value = entry.target.id
        }
      })
    },
    { threshold: 0.6 }
  )

  sections.forEach((section) => observer.observe(section))
})
</script>

<template>
  <header
    class="bg-blue-500 text-white sticky top-0 z-50 shadow-md"
  >
    <div class="container mx-auto px-4 py-3 flex flex-wrap justify-between items-center">
      <!-- Logo with White Background -->
      <div class="flex items-center bg-white rounded-full p-1">
        <img
          :src="logo_cropped"
          alt="Company Logo"
          class="h-16 w-auto"
        />
      </div>

      <!-- Mobile menu toggle -->
      <button
        class="md:hidden p-2 rounded border border-white hover:bg-blue-600 transition-colors"
        aria-label="Toggle navigation menu"
        @click="isToggle = !isToggle"
      >
        <i class="fas fa-bars text-xl"></i>
      </button>

      <!-- Navigation -->
      <nav
        class="w-full mt-4 md:mt-0 md:w-auto md:flex md:items-center"
        :class="{ 'block': isToggle, 'hidden': !isToggle }"
      >
        <ul class="flex flex-col md:flex-row items-center md:space-x-6 space-y-3 md:space-y-0 text-center">
          <li>
            <button
              @click="scrollToSection('home')"
              :class="{
                'text-yellow-300 font-semibold': activeSection === 'home',
                'hover:text-yellow-300': activeSection !== 'home'
              }"
              class="transition-colors duration-200"
            >
              Home
            </button>
          </li>
          <li>
            <button
              @click="scrollToSection('about')"
              :class="{
                'text-yellow-300 font-semibold': activeSection === 'about',
                'hover:text-yellow-300': activeSection !== 'about'
              }"
              class="transition-colors duration-200"
            >
              About
            </button>
          </li>
          <li>
            <button
              @click="scrollToSection('services')"
              :class="{
                'text-yellow-300 font-semibold': activeSection === 'services',
                'hover:text-yellow-300': activeSection !== 'services'
              }"
              class="transition-colors duration-200"
            >
              Services
            </button>
          </li>
          <li>
            <button
              @click="scrollToSection('team')"
              :class="{
                'text-yellow-300 font-semibold': activeSection === 'team',
                'hover:text-yellow-300': activeSection !== 'team'
              }"
              class="transition-colors duration-200"
            >
              Team
            </button>
          </li>
          <li>
            <button
              @click="scrollToSection('contact')"
              :class="{
                'text-yellow-300 font-semibold': activeSection === 'contact',
                'hover:text-yellow-300': activeSection !== 'contact'
              }"
              class="transition-colors duration-200"
            >
              Contact
            </button>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>