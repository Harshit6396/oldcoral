<template>
  <fixedheader/>
  <div class="relative min-h-screen">
    <!-- Background Image -->
    <div
        class="absolute inset-0 bg-cover bg-center bg-no-repeat opacity-20"
        style="background-image: url('/faq.jpg')"
    ></div>

    <!-- Content -->
    <div class="relative z-10">
      <!-- Header Section -->
      <div class="bg-slate-600 py-16 px-4">
        <div class="max-w-4xl mx-auto text-center">
          <h1 class="text-4xl md:text-5xl font-bold text-white">
            FAQ'S (FREQUENTLY ASKED QUESTIONS)
          </h1>
        </div>
      </div>

      <!-- FAQ Items -->
      <div class="max-w-4xl mx-auto py-12 px-4">
        <div class="space-y-4">
          <div
              v-for="(faq, index) in faqs"
              :key="index"
              class="bg-white rounded-lg shadow-sm border border-gray-200"
          >
            <!-- Question Header -->
            <button
                @click="toggleFAQ(index)"
                class="w-full px-6 py-4 text-left flex items-center justify-between hover:bg-gray-50 transition-colors duration-200"
            >
              <h3 class="text-lg font-medium text-gray-800 pr-4">
                {{ faq.question }}
              </h3>

              <!-- Toggle Button -->
              <div class="flex-shrink-0 hover:cursor-pointer">
                <div class="w-10 h-10 bg-blue-600 rounded-full flex items-center justify-center text-white font-bold text-xl transition-transform duration-200"
                     :class="{ 'rotate-180': faq.isOpen }">
                  {{ faq.isOpen ? '−' : '+' }}
                </div>
              </div>
            </button>

            <!-- Answer Content -->
            <Transition
                enter-active-class="transition-all duration-300 ease-out"
                enter-from-class="opacity-0 max-h-0"
                enter-to-class="opacity-100 max-h-96"
                leave-active-class="transition-all duration-300 ease-in"
                leave-from-class="opacity-100 max-h-96"
                leave-to-class="opacity-0 max-h-0"
            >
              <div v-if="faq.isOpen" class="overflow-hidden">
                <div class="px-6 pb-6 pt-2">
                  <p class="text-gray-600 leading-relaxed">
                    {{ faq.answer }}
                  </p>
                </div>
              </div>
            </Transition>
          </div>
        </div>
      </div>
    </div>
  </div>
  <Footer/>
</template>

<script setup>
import { ref, reactive } from 'vue'

// FAQ data with reactive state
const faqs = reactive([
  {
    question: "WHO SHALL BE IN-CHARGE OF MY PROJECT?",
    answer: "Coral Knowledge Services has a team of dedicated coders, document specialists, reviewers, data entry operators, solicitors, and web researchers who come here with diversified industry experience ready to host and serve all your needs. Depending on the type of project, these people would make sure their client is completely satisfied with the services. You shall be put in communication with one of the project managers as well.",
    isOpen: false
  },
  {
    question: "WHAT KIND OF SERVICES DOES CORAL KNOWLEDGE SERVICES PROVIDE?",
    answer: "We provide a comprehensive range of services including technical publications, translation services, transcription services, interpreting services, audio visual services, and data capture services. Our team is equipped to handle projects of various scales and complexities.",
    isOpen: false
  },
  {
    question: "WHAT ABOUT MY PRIVACY AND SECURITY CONCERNS?",
    answer: "We take privacy and security very seriously. All client data is handled with strict confidentiality agreements, secure data transmission protocols, and industry-standard security measures. Your information is protected throughout the entire project lifecycle.",
    isOpen: false
  },
  {
    question: "WHAT IS THE PROCEDURE TO MAKE THE PAYMENT?",
    answer: "We offer flexible payment options including bank transfers, online payments, and installment plans for larger projects. Payment terms are discussed and agreed upon before project commencement, with clear milestones and deliverables outlined.",
    isOpen: false
  },
  {
    question: "WILL YOU BE CITING THE AUTHORITIES IN YOUR RESEARCH AND PROVIDE ME A COPY?",
    answer: "Yes, absolutely. All our research work includes proper citations and references to authoritative sources. We provide complete documentation of all sources used, and you will receive copies of all relevant materials as part of your project deliverables.",
    isOpen: false
  },
  {
    question: "CAN I GET A SAMPLE PROJECT DONE, WILL IT BE FREE?",
    answer: "We offer sample work for evaluation purposes on a case-by-case basis. For smaller projects, we may provide a limited sample at no cost. For larger projects, we can discuss sample work as part of the project proposal process.",
    isOpen: false
  },
  {
    question: "IS THERE SOME SERVICE LEVEL AGREEMENT YOU SIGN WITH THE CLIENT?",
    answer: "Yes, we provide detailed Service Level Agreements (SLA) that outline project scope, timelines, quality standards, communication protocols, and deliverables. This ensures clear expectations and accountability for both parties.",
    isOpen: false
  },
  {
    question: "HOW CAN I CONTACT YOU?",
    answer: "You can contact us through multiple channels: email, phone, live chat on our website, or through our contact form. We also provide dedicated project managers for ongoing communication throughout your project.",
    isOpen: false
  },
  {
    question: "I STILL HAVE SOME QUERIES",
    answer: "No problem! We're here to help. Please don't hesitate to reach out to us with any additional questions. Our customer support team is available to address all your concerns and provide detailed information about our services.",
    isOpen: false
  }
])

// Toggle function
const toggleFAQ = (index) => {
  faqs[index].isOpen = !faqs[index].isOpen
}
</script>

<style scoped>
.max-h-96 {
  max-height: 24rem;
}

.max-h-0 {
  max-height: 0;
}
</style>
