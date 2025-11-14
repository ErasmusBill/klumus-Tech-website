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

    <!-- Main Content Container -->
    <div class="max-w-6xl mx-auto flex flex-col md:flex-row items-center gap-8 md:gap-12 mb-16">
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
        <p class="text-gray-700 text-lg leading-relaxed mb-6">
          At <span class="font-bold text-blue-600">KLUMUS Technologies</span>, we are a team of innovators transforming ideas into advanced digital solutions. We deliver high-quality, customer-focused services across web development, mobile apps, cloud computing, and AI technologies—combining creativity and technology to build functional, user-centered, and impactful solutions.
        </p>
        
        <p class="text-gray-700 text-lg leading-relaxed">
          Founded with a passion for excellence, we partner with businesses of all sizes to navigate the digital landscape. Our agile approach ensures we adapt to your unique needs while maintaining the highest standards of quality and innovation.
        </p>
        
        <div class="mt-8">
          <a 
            href="#contact" 
            class="inline-block bg-blue-600 text-white font-semibold px-8 py-3 rounded-lg shadow-lg hover:bg-blue-700 hover:shadow-xl transition-all duration-300 hover:-translate-y-1"
          >
            Partner With Us
          </a>
        </div>
      </div>
    </div>

    <!-- Mission & Vision -->
    <div class="max-w-6xl mx-auto grid md:grid-cols-2 gap-8 mb-16">
      <!-- Mission -->
      <div class="bg-white rounded-xl shadow-lg p-8 hover:shadow-2xl transition-shadow duration-300">
        <div class="flex items-center mb-4">
          <div class="w-12 h-12 bg-blue-100 rounded-lg flex items-center justify-center mr-4">
            <svg class="w-6 h-6 text-blue-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z"></path>
            </svg>
          </div>
          <h2 class="text-2xl font-bold text-gray-800">Our Mission</h2>
        </div>
        <p class="text-gray-600 leading-relaxed">
          To empower businesses through innovative technology solutions that drive growth, efficiency, and digital transformation. We strive to be the trusted partner that turns visionary ideas into reality, one project at a time.
        </p>
      </div>

      <!-- Vision -->
      <div class="bg-white rounded-xl shadow-lg p-8 hover:shadow-2xl transition-shadow duration-300">
        <div class="flex items-center mb-4">
          <div class="w-12 h-12 bg-purple-100 rounded-lg flex items-center justify-center mr-4">
            <svg class="w-6 h-6 text-purple-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 12a3 3 0 11-6 0 3 3 0 016 0z"></path>
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M2.458 12C3.732 7.943 7.523 5 12 5c4.478 0 8.268 2.943 9.542 7-1.274 4.057-5.064 7-9.542 7-4.477 0-8.268-2.943-9.542-7z"></path>
            </svg>
          </div>
          <h2 class="text-2xl font-bold text-gray-800">Our Vision</h2>
        </div>
        <p class="text-gray-600 leading-relaxed">
          To become a leading force in global digital innovation, recognized for our commitment to excellence, creativity, and transformative solutions that shape the future of technology and business.
        </p>
      </div>
    </div>

    <!-- Core Values -->
    <div class="max-w-6xl mx-auto mb-16">
      <h2 class="text-3xl font-bold text-gray-800 text-center mb-10">Our Core Values</h2>
      <div class="grid md:grid-cols-4 gap-6">
        <!-- Innovation -->
        <div class="bg-white rounded-xl p-6 text-center hover:shadow-xl transition-all duration-300 hover:-translate-y-2">
          <div class="w-16 h-16 bg-blue-100 rounded-full flex items-center justify-center mx-auto mb-4">
            <svg class="w-8 h-8 text-blue-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.663 17h4.673M12 3v1m6.364 1.636l-.707.707M21 12h-1M4 12H3m3.343-5.657l-.707-.707m2.828 9.9a5 5 0 117.072 0l-.548.547A3.374 3.374 0 0014 18.469V19a2 2 0 11-4 0v-.531c0-.895-.356-1.754-.988-2.386l-.548-.547z"></path>
            </svg>
          </div>
          <h3 class="text-xl font-bold text-gray-800 mb-2">Innovation</h3>
          <p class="text-gray-600 text-sm">Constantly pushing boundaries to deliver cutting-edge solutions</p>
        </div>

        <!-- Excellence -->
        <div class="bg-white rounded-xl p-6 text-center hover:shadow-xl transition-all duration-300 hover:-translate-y-2">
          <div class="w-16 h-16 bg-green-100 rounded-full flex items-center justify-center mx-auto mb-4">
            <svg class="w-8 h-8 text-green-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 12l2 2 4-4M7.835 4.697a3.42 3.42 0 001.946-.806 3.42 3.42 0 014.438 0 3.42 3.42 0 001.946.806 3.42 3.42 0 013.138 3.138 3.42 3.42 0 00.806 1.946 3.42 3.42 0 010 4.438 3.42 3.42 0 00-.806 1.946 3.42 3.42 0 01-3.138 3.138 3.42 3.42 0 00-1.946.806 3.42 3.42 0 01-4.438 0 3.42 3.42 0 00-1.946-.806 3.42 3.42 0 01-3.138-3.138 3.42 3.42 0 00-.806-1.946 3.42 3.42 0 010-4.438 3.42 3.42 0 00.806-1.946 3.42 3.42 0 013.138-3.138z"></path>
            </svg>
          </div>
          <h3 class="text-xl font-bold text-gray-800 mb-2">Excellence</h3>
          <p class="text-gray-600 text-sm">Committed to the highest standards in everything we do</p>
        </div>

        <!-- Integrity -->
        <div class="bg-white rounded-xl p-6 text-center hover:shadow-xl transition-all duration-300 hover:-translate-y-2">
          <div class="w-16 h-16 bg-yellow-100 rounded-full flex items-center justify-center mx-auto mb-4">
            <svg class="w-8 h-8 text-yellow-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 15v2m-6 4h12a2 2 0 002-2v-6a2 2 0 00-2-2H6a2 2 0 00-2 2v6a2 2 0 002 2zm10-10V7a4 4 0 00-8 0v4h8z"></path>
            </svg>
          </div>
          <h3 class="text-xl font-bold text-gray-800 mb-2">Integrity</h3>
          <p class="text-gray-600 text-sm">Building trust through transparency and honest communication</p>
        </div>

        <!-- Collaboration -->
        <div class="bg-white rounded-xl p-6 text-center hover:shadow-xl transition-all duration-300 hover:-translate-y-2">
          <div class="w-16 h-16 bg-purple-100 rounded-full flex items-center justify-center mx-auto mb-4">
            <svg class="w-8 h-8 text-purple-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17 20h5v-2a3 3 0 00-5.356-1.857M17 20H7m10 0v-2c0-.656-.126-1.283-.356-1.857M7 20H2v-2a3 3 0 015.356-1.857M7 20v-2c0-.656.126-1.283.356-1.857m0 0a5.002 5.002 0 019.288 0M15 7a3 3 0 11-6 0 3 3 0 016 0zm6 3a2 2 0 11-4 0 2 2 0 014 0zM7 10a2 2 0 11-4 0 2 2 0 014 0z"></path>
            </svg>
          </div>
          <h3 class="text-xl font-bold text-gray-800 mb-2">Collaboration</h3>
          <p class="text-gray-600 text-sm">Working together to achieve extraordinary results</p>
        </div>
      </div>
    </div>

    <!-- Statistics -->
    <div class="max-w-6xl mx-auto bg-gradient-to-r from-blue-600 to-purple-600 rounded-2xl shadow-2xl p-12">
      <h2 class="text-3xl font-bold text-white text-center mb-10">Our Impact in Numbers</h2>
      <div class="grid grid-cols-2 md:grid-cols-4 gap-8">
        <div class="text-center">
          <div class="text-4xl md:text-5xl font-bold text-white mb-2">20+</div>
          <div class="text-blue-100 text-sm md:text-base">Projects Delivered</div>
        </div>
        <div class="text-center">
          <div class="text-4xl md:text-5xl font-bold text-white mb-2">98%</div>
          <div class="text-blue-100 text-sm md:text-base">Client Satisfaction</div>
        </div>
        <!-- <div class="text-center">
          <div class="text-4xl md:text-5xl font-bold text-white mb-2">50+</div>
          <div class="text-blue-100 text-sm md:text-base">Happy Clients</div>
        </div> -->
        <div class="text-center">
          <div class="text-4xl md:text-5xl font-bold text-white mb-2">24/7</div>
          <div class="text-blue-100 text-sm md:text-base">Support Available</div>
        </div>
      </div>
    </div>
  </section>
</template>