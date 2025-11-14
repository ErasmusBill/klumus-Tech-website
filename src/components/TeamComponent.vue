<script setup>
import { ref } from 'vue'
import jibril from '@/assets/jibril.jpg'
import gideon1 from '@/assets/gideon1.jpg'
import khelly from '@/assets/khelly.jpg'
import desmond3 from '@/assets/desmond3.JPG'
import claudia from '@/assets/claudia.jpg'

const teamMembers = [
  {
    name: "Erasmus Charway Mensah",
    role: "CEO/Software Engineer/Lead Developer",
    photo: "khelly",
    bio: "Erasmus is the visionary leader behind our company with years of experience in the tech industry. He is also the mastermind of our web development and AI projects."
  },
  {
    name: "Gideon Amanor Tetteh",
    role: "CTO",
    photo: "gideon1",
    bio: "Gideon is our tech guru, leading the development team with innovative solutions and cutting-edge technology."
  },
  {
    name: "Bonages Kwabena Bonfil",
    role: "CFO",
    photo: "jibril",
    bio: "Bonages manages our financial strategies ensuring sustainable growth and profitability."
  },
  {
    name: "Claudia Bartels",
    role: "Project Manager/HR",
    photo: "claudia",
    bio: "Claudia coordinates our projects, ensuring timely delivery and client satisfaction."
  },
  {
    name: "Desmond Bortey",
    role: "Lead Designer",
    photo: "desmond3",
    bio: "Kelly brings creativity to our team, crafting visually stunning designs that captivate our clients."
  }
]

const getPhotoSrc = (photo) => {
  const photoMap = { jibril, gideon1, khelly, claudia,desmond3 }
  return photoMap[photo] || photo
}
</script>

<template>
  <section class="bg-gradient-to-br from-gray-50 to-gray-100 py-16 px-4">
    <!-- Header -->
    <div class="max-w-7xl mx-auto text-center mb-12">
      <h1 class="text-4xl md:text-5xl font-bold text-gray-800 mb-4">
        Meet Our Team
      </h1>
      <p class="text-gray-600 text-lg max-w-2xl mx-auto">
        The talented people behind our success
      </p>
    </div>

    <!-- Team Members Container -->
    <div class="max-w-7xl mx-auto flex flex-wrap justify-center gap-8">
      <div 
        v-for="member in teamMembers" 
        :key="member.name" 
        class="bg-white rounded-2xl shadow-lg p-8 text-center transition-all duration-300 hover:shadow-2xl hover:-translate-y-2 w-full sm:w-80 md:w-72 lg:w-80"
      >
        <!-- Photo with hover effect -->
        <div class="mb-6 relative inline-block">
          <img
            :src="getPhotoSrc(member.photo)"
            :alt="member.name"
            class="w-32 h-32 rounded-full object-cover border-4 border-blue-100 transition-transform duration-300 hover:scale-105 hover:border-blue-300"
          />
          <div class="absolute inset-0 rounded-full bg-blue-500 opacity-0 hover:opacity-10 transition-opacity duration-300"></div>
        </div>

        <!-- Name -->
        <h2 class="text-xl font-bold text-gray-800 mb-2">
          {{ member.name }}
        </h2>

        <!-- Role -->
        <p class="text-blue-600 font-semibold mb-4 text-sm uppercase tracking-wide">
          {{ member.role }}
        </p>

        <!-- Bio -->
        <p class="text-gray-600 leading-relaxed text-sm">
          {{ member.bio }}
        </p>
      </div>
    </div>
  </section>
</template>