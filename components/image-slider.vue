<template>
  <div class="relative w-full h-96 md:h-[500px] overflow-hidden bg-gray-100">
    <!-- Slides -->
    <div class="relative w-full h-full">
      <div
          v-for="(slide, index) in slides"
          :key="slide.id"
          :class="`absolute inset-0 transition-opacity duration-1000 ease-in-out ${
          index === currentSlide ? 'opacity-100' : 'opacity-0'
        }`"
      >
        <!-- Use regular <img> tag instead of NuxtImg -->
        <img
            :src="slide.src"
            :alt="slide.alt"
            class="w-full h-full object-cover"
            :loading="index === 0 ? 'eager' : 'lazy'"
        />
        <!-- Overlay with content -->
        <div class="absolute inset-0 bg-opacity-40 flex items-center justify-center">
          <div class="text-center text-white px-4 max-w-2xl">
            <!-- Title and Description with separation -->
            <h2 class="text-3xl md:text-4xl font-bold mb-4 text-black">{{ slide.title }}</h2>
            <p class="text-lg md:text-xl opacity-90 text-white">{{ slide.description }}</p> <!-- Change text color to white -->
          </div>
        </div>
      </div>
    </div>

    <!-- Navigation Arrows -->
    <button
        @click="prevSlide"
        class="absolute left-4 top-1/2 transform -translate-y-1/2 bg-gray-800 hover:bg-black text-white p-2 rounded-full transition-all duration-200 cursor-pointer"
        aria-label="Previous slide"
    >
      <svg class="w-6 h-6 font-bold" fill="none" stroke="currentColor" viewBox="0 0 24 24">
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 19l-7-7 7-7" />
      </svg>
    </button>

    <button
        @click="nextSlide"
        class="absolute right-4 top-1/2 transform -translate-y-1/2 bg-gray-800 hover:bg-black text-white p-2 rounded-full transition-all duration-200 cursor-pointer"
        aria-label="Next slide"
    >
      <svg class="w-6 h-6 font-bold" fill="none" stroke="currentColor" viewBox="0 0 24 24">
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7" />
      </svg>
    </button>

    <!-- Dots Navigation -->
    <div class="absolute bottom-4 left-1/2 transform -translate-x-1/2 flex space-x-2">
      <button
          v-for="(slide, index) in slides"
          :key="index"
          @click="goToSlide(index)"
          :class="`w-3 h-3 rounded-full transition-all duration-200 ${
          index === currentSlide ? 'bg-white' : 'bg-white bg-opacity-50 hover:bg-opacity-75'
        }`"
          :aria-label="`Go to slide ${index + 1}`"
      />
    </div>
  </div>
</template>

<script setup>
import { ref, onMounted, onUnmounted } from 'vue'

const slides = [
  {
    id: 1,
    src: "/slide1.jpg",  // Correct path to the first image in the public folder
    alt: "Certified Translations illustration",
    title: "Certified Translations You Can Trust",
    description: "Coral provides certified, accredited translation services for medical, financial, and legal, as well as government and official documents.",
  },
  {
    id: 2,
    src: "/slide2.jpg",  // Correct path to the second image in the public folder
    alt: "Professional using mobile device for communication",
    title: "OUR TECHNOLOGY AND PROCESS WILL ENABLE YOU TO CUT COSTS, TIME AND MARKETS FASTER",
    description: "Get products to global market faster ",
  },
  {
    id: 3,
    src: "/slide3.jpg",  // Correct path to the third image in the public folder
    alt: "Vintage bicycle representing simplicity and efficiency",
    title: "Simple & Efficient International Market",
    description: "Learn more about the solutions that we have for you",
  },
]

const currentSlide = ref(0)
let timer = null

// Auto-play functionality
onMounted(() => {
  timer = setInterval(() => {
    currentSlide.value = (currentSlide.value + 1) % slides.length
  }, 5000) // Change slide every 5 seconds
})

onUnmounted(() => {
  if (timer) {
    clearInterval(timer)
  }
})

const goToSlide = (index) => {
  currentSlide.value = index
}

const nextSlide = () => {
  currentSlide.value = (currentSlide.value + 1) % slides.length
}

const prevSlide = () => {
  currentSlide.value = (currentSlide.value - 1 + slides.length) % slides.length
}
</script>


<style>
p.text-lg.md\:text-xl.opacity-90.text-white {
  color: #221c1cd6;
}


</style>
