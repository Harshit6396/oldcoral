
<template>
  <h2 class="text-xl mb-10 tracking-wider text-center">GET IN TOUCH</h2>
  <section class="relative">
    <!-- Get In Touch Hero Section -->
    <div
        class="relative min-h-96 bg-cover bg-center bg-no-repeat"
        :style="{ backgroundImage: 'url(https://i.ibb.co/8DnWBQH2/getintouch.jpg)' }">

      <!-- Dark overlay -->
      <div class="absolute inset-0 bg-opacity-60"></div>

      <!-- Content with padding -->
      <div class="relative z-10 flex flex-col items-center justify-center h-full text-white p-[121px]">

        <!-- Overlay -->
        <div class="absolute inset-0 bg-black opacity-50 z-0"></div> <!-- This is your overlay -->

        <!-- Social Media Icons -->
        <div class="flex flex-wrap justify-center gap-10 max-w-4xl z-10">
          <!-- Twitter -->
          <div class="flex flex-col items-center">
            <a href="https://x.com/rahulchhillar" target="_blank" class="w-24 h-24 rounded-full border-2 border-white flex items-center justify-center mb-3 hover:bg-white hover:text-black transition-colors cursor-pointer">
              <svg class="w-12 h-12" fill="currentColor" viewBox="0 0 24 24">
                <path d="M23.953 4.57a10 10 0 01-2.825.775 4.958 4.958 0 002.163-2.723c-.951.555-2.005.959-3.127 1.184a4.92 4.92 0 00-8.384 4.482C7.69 8.095 4.067 6.13 1.64 3.162a4.822 4.822 0 00-.666 2.475c0 1.71.87 3.213 2.188 4.096a4.904 4.904 0 01-2.228-.616v.06a4.923 4.923 0 003.946 4.827 4.996 4.996 0 01-2.212.085 4.936 4.936 0 004.604 3.417 9.867 9.867 0 01-6.102 2.105c-.39 0-.779-.023-1.17-.067a13.995 13.995 0 007.557 2.209c9.053 0 13.998-7.496 13.998-13.985 0-.21 0-.42-.015-.63A9.935 9.935 0 0024 4.59z"/>
              </svg>
            </a>
            <p class="text-sm text-center">
              <span class="block text-xs opacity-80 text-white">Follow Us on</span>
              <span class="font-semibold text-white">TWITTER</span>
            </p>
          </div>

          <!-- Facebook -->
          <div class="flex flex-col items-center">
            <a href="https://www.facebook.com/coralknowledgeservices" target="_blank" class="w-24 h-24 rounded-full border-2 border-white flex items-center justify-center mb-3 hover:bg-white hover:text-black transition-colors cursor-pointer">
              <svg class="w-12 h-12" fill="currentColor" viewBox="0 0 24 24">
                <path d="M24 12.073c0-6.627-5.373-12-12-12s-12 5.373-12 12c0 5.99 4.388 10.954 10.125 11.854v-8.385H7.078v-3.47h3.047V9.43c0-3.007 1.792-4.669 4.533-4.669 1.312 0 2.686.235 2.686.235v2.953H15.83c-1.491 0-1.956.925-1.956 1.874v2.25h3.328l-.532 3.47h-2.796v8.385C19.612 23.027 24 18.062 24 12.073z"/>
              </svg>
            </a>
            <p class="text-sm text-center">
              <span class="block text-xs opacity-80 text-white">Like Us at</span>
              <span class="font-semibold text-white">FACEBOOK</span>
            </p>
          </div>

          <!-- LinkedIn -->
          <div class="flex flex-col items-center">
            <a href="https://www.linkedin.com/in/rahulchhillar/" target="_blank" class="w-24 h-24 rounded-full border-2 border-white flex items-center justify-center mb-3 hover:bg-white hover:text-black transition-colors cursor-pointer">
              <svg class="w-12 h-12" fill="currentColor" viewBox="0 0 24 24">
                <path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433c-1.144 0-2.063-.926-2.063-2.065 0-1.138.92-2.063 2.063-2.063 1.14 0 2.064.925 2.064 2.063 0 1.139-.925 2.065-2.064 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/>
              </svg>
            </a>
            <p class="text-sm text-center">
              <span class="block text-xs opacity-80 text-white">Connect With Us at</span>
              <span class="font-semibold text-white">LINKEDIN</span>
            </p>
          </div>

          <!-- Google Plus -->
          <div class="flex flex-col items-center">
            <a href="https://workspaceupdates.googleblog.com/2023/04/new-community-features-for-google-chat-and-an-update-currents%20.html" target="_blank" class="w-24 h-24 rounded-full border-2 border-white flex items-center justify-center mb-3 hover:bg-white hover:text-black transition-colors cursor-pointer">
              <svg class="w-12 h-12" fill="currentColor" viewBox="0 0 24 24">
                <path d="M7.635 10.909v2.619h4.335c-.173 1.125-1.31 3.295-4.335 3.295-2.512 0-4.57-2.085-4.57-4.66 0-2.575 2.058-4.66 4.57-4.66 1.431 0 2.387.609 2.943 1.133l2.06-1.985C10.462 4.668 9.1 4 7.635 4c-4.106 0-7.435 3.331-7.435 7.435s3.329 7.435 7.435 7.435c4.29 0 7.135-3.015 7.135-7.26 0-.488-.054-.858-.12-1.225H7.635z"/>
                <path d="M24 10.909h-2.182V8.727h-2.182v2.182h-2.182v2.182h2.182v2.182h2.182v-2.182H24v-2.182z"/>
              </svg>
            </a>
            <p class="text-sm text-center">
              <span class="block text-xs opacity-80 text-white">Explore Us on</span>
              <span class="font-semibold text-white">GOOGLE PLUS</span>
            </p>
          </div>
        </div>
      </div>

    </div>
  </section>

  <!-- Logo Section  -->
  <section class="bg-gray-50 py-8">
    <div class="w-full px-4">
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
