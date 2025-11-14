<template>
  <section class="bg-gradient-to-br from-blue-500 via-blue-600 to-blue-700 text-white w-full min-h-screen py-10 px-4">
    <div class="max-w-7xl mx-auto">
      <!-- Header -->
      <div class="text-center mb-10">
        <h1 class="text-4xl md:text-5xl lg:text-6xl font-bold mb-3">Get In Touch</h1>
        <p class="text-lg md:text-xl text-blue-100 max-w-2xl mx-auto">
          We'd love to hear from you. Send us a message and we'll respond as soon as possible.
        </p>
      </div>

      <div class="grid lg:grid-cols-2 gap-8 lg:gap-12">
        <!-- LEFT column -->
        <div class="space-y-6">

          <!-- Contact Info -->
          <div class="bg-white/10 backdrop-blur-lg rounded-2xl p-6 shadow-xl">
            <h2 class="text-2xl font-semibold mb-4 flex items-center gap-2">
              <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                  d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z" />
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                  d="M15 11a3 3 0 11-6 0 3 3 0 016 0z" />
              </svg>
              Contact Information
            </h2>

            <div class="space-y-3 text-blue-50">
              <p class="flex items-start gap-3">
                <span class="font-semibold min-w-[80px]">Address:</span>
                <span>Omanu Beach, Nungua<br />Greater Accra Region<br />Ghana 🇬🇭</span>
              </p>

              <p class="flex items-start gap-3">
                <span class="font-semibold min-w-[80px]">Phone:</span>
                <span>
                  <a href="tel:+233501234567" class="hover:underline">+233 (0) 59 684 4242</a><br />
                  <a href="tel:+233241234567" class="hover:underline">+233 (0) 54 050 1163</a>
                </span>
              </p>

              <p class="flex items-start gap-3">
                <span class="font-semibold min-w-[80px]">Email:</span>
                <span>
                  <a href="mailto:info@example.com" class="hover:underline">info@klumustechnologies.com</a>
                </span>
              </p>
            </div>
          </div>

          <!-- Social Media -->
          <div class="bg-white/10 backdrop-blur-lg rounded-2xl p-6 shadow-xl">
            <h2 class="text-2xl font-semibold mb-4 flex items-center gap-2">
              <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                  d="M17 20h5v-2a3 3 0 00-5.356-1.857M17 20H7m10 0v-2c0-.656-.126-1.283-.356-1.857M7 20H2v-2a3 3 0 015.356-1.857M7 20v-2c0-.656.126-1.283.356-1.857m0 0a5.002 5.002 0 019.288 0M15 7a3 3 0 11-6 0 3 3 0 016 0zm6 3a2 2 0 11-4 0 2 2 0 014 0zM7 10a2 2 0 11-4 0 2 2 0 014 0z" />
              </svg>
              Connect With Us
            </h2>

            <p class="text-blue-100 text-sm mb-4">Follow us on social media for updates</p>

            <div class="flex flex-wrap gap-3">
              <!-- Facebook -->
              <a :href="socialLinks.facebook" target="_blank"
                class="flex items-center justify-center w-12 h-12 bg-white/20 hover:bg-white/30 rounded-xl transition-all hover:scale-110">
                <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                  <path
                    d="M24 12.073c0-6.627-5.373-12-12-12s-12 5.373-12 12c0 5.99 4.388 10.954 10.125 11.854v-8.385H7.078v-3.47h3.047V9.43c0-3.007 1.792-4.669 4.533-4.669 1.312 0 2.686.235 2.686.235v2.953H15.83c-1.491 0-1.956.925-1.956 1.874v2.25h3.328l-.532 3.47h-2.796v8.385C19.612 23.027 24 18.062 24 12.073z" />
                </svg>
              </a>

              <!-- Twitter -->
              <a :href="socialLinks.twitter" target="_blank"
                class="flex items-center justify-center w-12 h-12 bg-white/20 hover:bg-white/30 rounded-xl transition-all hover:scale-110">
                <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                  <path
                    d="M18.244 2.25h3.308l-7.227 8.26 8.502 11.24H16.17l-5.214-6.817L4.99 21.75H1.68l7.73-8.835L1.254 2.25H8.08l4.713 6.231zm-1.161 17.52h1.833L7.084 4.126H5.117z" />
                </svg>
              </a>

              <!-- Instagram -->
              <a :href="socialLinks.instagram" target="_blank"
                class="flex items-center justify-center w-12 h-12 bg-white/20 hover:bg-white/30 rounded-xl transition-all hover:scale-110">
                <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                  <path
                    d="M12 2.163c3.204 0 3.584.012 4.85.07 3.252.148 4.771 1.691 4.919 4.919.058 1.265.069 1.645.069 4.849 0 3.205-.012 3.584-.069 4.849-.149 3.225-1.664 4.771-4.919 4.919-1.266.058-1.644.07-4.85.07-3.204 0-3.584-.012-4.849-.07-3.26-.149-4.771-1.699-4.919-4.92-.058-1.265-.07-1.644-.07-4.849 0-3.204.013-3.583.07-4.849.149-3.227 1.664-4.771 4.919-4.919 1.266-.057 1.645-.069 4.849-.069z" />
                </svg>
              </a>

              <!-- LinkedIn -->
              <a :href="socialLinks.linkedin" target="_blank"
                class="flex items-center justify-center w-12 h-12 bg-white/20 hover:bg-white/30 rounded-xl transition-all hover:scale-110">
                <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                  <path
                    d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433c-1.144 0-2.063-.926-2.063-2.065 0-1.138.92-2.063 2.063-2.063 1.14 0 2.064.925 2.064 2.063 0 1.139-.925 2.065-2.064 2.065zm1.782 13.019H3.555V9h3.564v11.452z" />
                </svg>
              </a>

              <!-- TikTok -->
              <a :href="socialLinks.tiktok" target="_blank"
                class="flex items-center justify-center w-12 h-12 bg-white/20 hover:bg-white/30 rounded-xl transition-all hover:scale-110">
                <svg class="w-6 h-6" fill="currentColor" viewBox="0 0 24 24">
                  <path
                    d="M19.59 6.69a4.83 4.83 0 01-3.77-4.25V2h-3.45v13.67a2.89 2.89 0 01-5.2 1.74 2.89 2.89 0 012.31-4.64 2.93 2.93 0 01.88.13V9.4a6.84 6.84 0 00-1-.05A6.33 6.33 0 005 20.1a6.34 6.34 0 0010.86-4.43v-7a8.16 8.16 0 004.77 1.52v-3.4a4.85 4.85 0 01-1-.1z" />
                </svg>
              </a>
            </div>
          </div>

          <!-- Map -->
          <div class="bg-white/10 backdrop-blur-lg rounded-2xl p-4 shadow-xl">
            <div id="osm-map" class="w-full h-80 md:h-96 rounded-xl shadow-md bg-gray-200"></div>
            <p class="mt-3 text-center text-sm text-blue-100">
              📍 Click the marker for more details
            </p>
          </div>
        </div>

        <!-- RIGHT column - Form -->
        <div class="bg-white/10 backdrop-blur-lg rounded-2xl p-6 md:p-8 shadow-xl">

          <h2 class="text-2xl font-semibold mb-6 flex items-center gap-2">
            <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                d="M3 8l7.89 5.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
            </svg>
            Send Us a Message
          </h2>

          <!-- Success -->
          <div v-if="submitSuccess"
            class="mb-6 p-4 bg-green-500/20 border border-green-400 rounded-lg flex items-start gap-3">
            <svg class="w-6 h-6 text-green-300 flex-shrink-0 mt-0.5" fill="none" stroke="currentColor"
              viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z" />
            </svg>
            <div>
              <p class="font-semibold text-green-100">Message sent successfully!</p>
              <p class="text-sm text-green-200">We'll get back to you soon.</p>
            </div>
          </div>

          <!-- Error -->
          <div v-if="submitError"
            class="mb-6 p-4 bg-red-500/20 border border-red-400 rounded-lg flex items-start gap-3">
            <svg class="w-6 h-6 text-red-300 flex-shrink-0 mt-0.5" fill="none" stroke="currentColor"
              viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                d="M12 8v4m0 4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
            </svg>
            <p class="text-red-100">{{ submitError }}</p>
          </div>

          <div class="space-y-5">
            <!-- Name -->
            <div>
              <label class="block text-sm font-medium mb-2">Your Name *</label>
              <input v-model="formData.name" type="text" required class="w-full px-4 py-3 rounded-lg text-gray-800" />
            </div>

            <!-- Email -->
            <div>
              <label class="block text-sm font-medium mb-2">Email *</label>
              <input v-model="formData.email" type="email" required class="w-full px-4 py-3 rounded-lg text-gray-800" />
            </div>

            <!-- Subject -->
            <div>
              <label class="block text-sm font-medium mb-2">Subject *</label>
              <input v-model="formData.subject" type="text" required class="w-full px-4 py-3 rounded-lg text-gray-800" />
            </div>

            <!-- Message -->
            <div>
              <label class="block text-sm font-medium mb-2">Your Message *</label>
              <textarea v-model="formData.message" rows="5" class="w-full px-4 py-3 rounded-lg text-gray-800"></textarea>
            </div>

            <!-- Submit -->
            <button @click="handleSubmit" :disabled="isSubmitting"
              class="w-full bg-white text-blue-600 font-semibold py-3.5 rounded-lg shadow-lg hover:bg-gray-50 flex items-center justify-center gap-2">
              <span v-if="isSubmitting" class="animate-spin w-5 h-5 border rounded-full border-t-transparent"></span>
              <span v-else>Send Message</span>
            </button>

          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
import { ref, onMounted } from "vue";
import L from "leaflet";

// SOCIAL LINKS
const socialLinks = ref({
  facebook: "#",
  twitter: "#",
  instagram: "#",
  linkedin: "#",
  tiktok: "#",
});

// FORM DATA
const formData = ref({
  name: "",
  email: "",
  subject: "",
  message: "",
});

const isSubmitting = ref(false);
const submitSuccess = ref(false);
const submitError = ref("");

// FORM SUBMIT
const handleSubmit = async () => {
  isSubmitting.value = true;
  submitError.value = "";
  submitSuccess.value = false;

  setTimeout(() => {
    if (!formData.value.name || !formData.value.email || !formData.value.message) {
      submitError.value = "Please fill all required fields.";
    } else {
      submitSuccess.value = true;
      formData.value = { name: "", email: "", subject: "", message: "" };
    }
    isSubmitting.value = false;
  }, 1200);
};

// LEAFLET MAP
onMounted(() => {
  const map = L.map("osm-map").setView([5.6017, -0.0787], 14);

  L.tileLayer("https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png").addTo(map);

  const marker = L.marker([5.6017, -0.0787]).addTo(map);
  marker.bindPopup("Omanu Beach, Nungua").openPopup();
});
</script>

<style>
.leaflet-container {
  background: #e0e0e0;
  border-radius: 0.75rem;
}
</style>
