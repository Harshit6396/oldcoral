<template>

  <!-- Logo Section  -->
  <section class="bg-gray-50 py-8">
    <div class="w-full px-4 text-center">
      <!-- Heading -->
      <h2 class="text-l font-semibold text-gray-800 mb-6">People We Have Worked With</h2>

      <div class="w-full">
        <div class="flex justify-center gap-10 flex-nowrap">
          <div class="w-auto">
            <img src="/public/the-smart-cube-logo.png" alt="The Smart Cube" class="w-full" />
          </div>
          <div class="w-auto">
            <img src="/public/E-n-y-logo.png" alt="EY" class="w-full" />
          </div>
          <div class="w-auto">
            <img src="/public/hwauei-logo.png" alt="Huawei" class="w-full" />
          </div>
          <div class="w-auto">
            <img src="/public/xaiomi.png" alt="Xiaomi" class="w-full" />
          </div>
          <div class="w-auto">
            <img src="/public/Tik-Tok.png" alt="TikTok" class="w-full" />
          </div>
          <div class="w-auto">
            <img src="/public/Tata.png" alt="Tata" class="w-full" />
          </div>
        </div>
      </div>
    </div>
  </section>





  <!-- Testimonials Section -->
  <div class="bg-white py-16">
    <div class="container mx-auto px-4 text-center">
      <h3 class="text-2xl font-bold text-gray-800 mb-8">WHAT PEOPLE SAY ABOUT US</h3>

      <div class="max-w-4xl mx-auto relative">
        <!-- Testimonial Slider -->
        <div class="overflow-hidden">
          <div
              class="flex transition-transform duration-500 ease-in-out"
              :style="{ transform: `translateX(-${currentSlide * 100}%)` }"
          >
            <!-- Slide 1 -->
            <div class="w-full flex-shrink-0 px-4">
              <blockquote class="text-gray-600 text-lg leading-relaxed mb-6">
                Rahul, as a team lead, has been instrumental in refining my professional skills though his style of stress free and inspirational team management. Majority of knowledge which I acquired at Evalueserve is a result of Rahul's continuous efforts to improve quality and imbibing a try-yourself culture.<br>
                Wishing you all the best for your future.
              </blockquote>

              <h3 class="cite text-sm text-gray-500">
                <span class="quote-name font-semibold">- Pratik Yadav</span>,
                <span class="quote-desc">Experienced Global Supply Chain & Logistics Professional</span>
              </h3>
            </div>

            <!-- Slide 2 -->
            <div class="w-full flex-shrink-0 px-4">
              <blockquote class="text-gray-600 text-lg leading-relaxed mb-6">
                The service received from Coral was very professional and prompt. The quality of the translation and reporting templates was outstanding and the language style was exactly what we were looking for.
              </blockquote>

              <h3 class="cite text-sm text-gray-500">
                <span class="quote-name font-semibold">- President</span>,
                <span class="quote-desc">Research Firm Based in USA</span>
              </h3>
            </div>

            <!-- Slide 3 (New Testimonial) -->
            <div class="w-full flex-shrink-0 px-4">
              <blockquote class="text-gray-600 text-lg leading-relaxed mb-6">
                Very smart people working on the project — they provided great insight and brought experience to the project. Project Management team was very prompt and the team was able to respond quickly to the changing project requirements.
              </blockquote>

              <h3 class="cite text-sm text-gray-500">
                <span class="quote-name font-semibold">- Manager</span>,
                <span class="quote-desc">Leading IT Company</span>
              </h3>
            </div>

            <!-- Slide 4 (New Testimonial) -->
            <div class="w-full flex-shrink-0 px-4">
              <blockquote class="text-gray-600 text-lg leading-relaxed mb-6">
                Rahul has very good analytical skills with “Never say die attitude” and always wants to learn more. He has very good grasping skills. He has a very helpful nature and always keeps smiling. He would go very high in the corporate ladder. I wish him the very best in all his endavours.
              </blockquote>

              <h3 class="cite text-sm text-gray-500">
                <span class="quote-name font-semibold">- Anand Lakshmanan</span>,
                <span class="quote-desc">National Collections Manager - SME Loans at Axis Bank Limited</span>
              </h3>
            </div>
          </div>
        </div>

        <!-- Navigation arrows -->
        <div class="flex justify-center gap-4 mt-8">
          <button
              @click="previousSlide"
              class="w-10 h-10 rounded-full border border-gray-300 flex items-center justify-center hover:bg-gray-100 transition-colors"
              :disabled="currentSlide === 0"
              :class="{ 'opacity-50 cursor-not-allowed': currentSlide === 0 }"
          >
            <svg class="w-5 h-5 text-gray-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 19l-7-7 7-7"/>
            </svg>
          </button>
          <button
              @click="nextSlide"
              class="w-10 h-10 rounded-full border border-gray-300 flex items-center justify-center hover:bg-gray-100 transition-colors"
              :disabled="currentSlide === testimonials.length - 1"
              :class="{ 'opacity-50 cursor-not-allowed': currentSlide === testimonials.length - 1 }"
          >
            <svg class="w-5 h-5 text-gray-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5l7 7-7 7"/>
            </svg>
          </button>
        </div>

        <!-- Slide indicators -->
        <div class="flex justify-center gap-2 mt-4">
          <button
              v-for="(_, index) in testimonials"
              :key="index"
              @click="goToSlide(index)"
              class="w-3 h-3 rounded-full transition-colors"
              :class="currentSlide === index ? 'bg-gray-600' : 'bg-gray-300'"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
import { ref, onMounted, onUnmounted } from 'vue'

interface Testimonial {
  quote: string
  name: string
  title: string
}

const testimonials: Testimonial[] = [
  {
    quote: "Rahul, as a team lead, has been instrumental in refining my professional skills though his style of stress free and inspirational team management. Majority of knowledge which I acquired at Evalueserve is a result of Rahul's continuous efforts to improve quality and imbibing a try-yourself culture. Wishing you all the best for your future.",
    name: "Pratik Yadav",
    title: "Experienced Global Supply Chain & Logistics Professional"
  },
  {
    quote: "The service received from Coral was very professional and prompt. The quality of the translation and reporting templates was outstanding and the language style was exactly what we were looking for.",
    name: "President",
    title: "Research Firm Based in USA"
  },
  {
    quote: "Very smart people working on the project — they provided great insight and brought experience to the project. Project Management team was very prompt and the team was able to respond quickly to the changing project requirements.",
    name: "Manager",
    title: "Leading IT Company"
  },
  {
    quote: "Rahul has very good analytical skills with “Never say die attitude” and always wants to learn more. He has very good grasping skills. He has a very helpful nature and always keeps smiling. He would go very high in the corporate ladder. I wish him the very best in all his endavours.",
    name: "Anand Lakshmanan",
    title: "National Collections Manager - SME Loans at Axis Bank Limited"
  }
]

const currentSlide = ref<number>(0)
let autoSlideInterval: NodeJS.Timeout | null = null

const nextSlide = (): void => {
  if (currentSlide.value < testimonials.length - 1) {
    currentSlide.value++
  } else {
    currentSlide.value = 0
  }
}

const previousSlide = (): void => {
  if (currentSlide.value > 0) {
    currentSlide.value--
  } else {
    currentSlide.value = testimonials.length - 1
  }
}

const goToSlide = (index: number): void => {
  currentSlide.value = index
}

const startAutoSlide = (): void => {
  autoSlideInterval = setInterval(() => {
    nextSlide()
  }, 5000) // Auto-slide every 5 seconds
}

const stopAutoSlide = (): void => {
  if (autoSlideInterval) {
    clearInterval(autoSlideInterval)
    autoSlideInterval = null
  }
}

onMounted(() => {
  startAutoSlide()
})

onUnmounted(() => {
  stopAutoSlide()
})
</script>

<style scoped>
.cite {
  font-style: italic;
}

.quote-name {
  color: #374151;
}

.quote-desc {
  color: #6b7280;
}
</style>
