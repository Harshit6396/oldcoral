<template>
  <Fixedheader/>
  <div class="min-h-screen bg-white">
    <!-- Header Section -->
    <section class="relative bg-cover bg-center py-30" style="background-image: url('/pro.jpg')">
      <!-- Overlay -->
      <div class="absolute inset-0 bg-[#34495e] opacity-75"></div>

      <!-- Content -->
      <div class="relative text-center text-white max-w-4xl mx-auto px-4">
        <h1 class="text-4xl font-semibold uppercase relative inline-block mb-4">
          THOUGHTS FROM CORAL
          <!-- Blue Underline under the text -->
          <div class="absolute bottom-0 left-0 w-full h-0.5 bg-blue-500"></div>
        </h1>
        <h2 class="text-xs mt-2 tracking-widest">
          LATEST TRENDS AND INSIGHTS IN THE TRANSLATION INDUSTRY
        </h2>
      </div>
    </section>


    <!-- Main Content and Sidebar -->
    <div class="container mx-auto px-6 pt-12 grid grid-cols-1 lg:grid-cols-4 gap-10 max-w-7xl">
      <!-- Blog Posts List -->
      <div class="lg:col-span-3 grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6">
        <article v-for="post in pagedPosts" :key="post.id" class="border border-gray-200 p-4 hover:shadow-md transition-shadow cursor-pointer">
          <p class="text-xs uppercase font-semibold text-blue-600 mb-2">{{ post.category }}</p>
          <h2 class="font-semibold text-sm mb-2 leading-snug">{{ post.title }}</h2>
          <p class="text-xs text-gray-500 line-clamp-3">{{ post.excerpt }}</p>
        </article>
      </div>

      <!-- Sidebar -->
      <aside class="hidden lg:block space-y-6">
        <!-- Search -->
        <div>
          <input
              v-model="searchTerm"
              type="search"
              placeholder="Search..."
              class="w-full border border-gray-300 px-3 py-2 rounded-md focus:outline-none focus:ring-2 focus:ring-blue-500"
          />
        </div>

        <!-- Recent Posts -->
        <div>
          <h3 class="uppercase text-xs font-semibold mb-2">Recent Posts</h3>
          <ul class="space-y-2 text-xs text-gray-600">
            <li v-for="post in recentPosts" :key="post.id" class="hover:text-blue-600 cursor-pointer" @click="goToPost(post.id)">
              {{ post.title }}
            </li>
          </ul>
        </div>
      </aside>
    </div>

    <!-- Pagination -->
    <div class="flex justify-center space-x-4 mt-12 mb-16">
      <!-- Previous Button -->
      <button
          @click="prevPage"
          :disabled="currentPage === 1"
          class="px-4 py-1 rounded bg-gray-200 disabled:opacity-50 hover:cursor-pointer"
      >
        Prev
      </button>

      <!-- Page Buttons -->
      <button
          v-for="page in totalPages"
          :key="page"
          @click="goToPage(page)"
          :class="[
      'px-4 py-1 rounded',
      page === currentPage ? 'bg-blue-600 text-white' : 'bg-gray-200',
      'hover:cursor-pointer'
    ]"
      >
        {{ page }}
      </button>

      <!-- Next Button -->
      <button
          @click="nextPage"
          :disabled="currentPage === totalPages"
          class="px-4 py-1 rounded bg-gray-200 disabled:opacity-50 hover:cursor-pointer"
      >
        Next
      </button>
    </div>
  </div>
  <Footer />
</template>

<script setup>
import { ref, computed } from 'vue'
import { useRouter } from 'vue-router'

// Sample blog posts data, replace with API calls or Markdown content as needed
const posts = ref([
  {
    id: 1,
    title: 'E-learning Translation - Attempt for an effective globalization',
    category: 'Translation',
    excerpt: 'In the enormous competitive world there are many national and multinational companies working for different domains. These days presence of ...'
  },
  {
    id: 2,
    title: 'Transcreation Gaining Momentum in the Translation Industry',
    category: 'Translation',
    excerpt: 'Transcreation is a process of adapting a creative piece of work into another language whilst maintaining its cultural impact. The ...'
  },
  {
    id: 3,
    title: 'Include Desktop Multilingual DTP for Effective Marketing Practices',
    category: 'Translation',
    excerpt: 'Multilingual DTP is used to make your documents look pretty, decent and really attractive. What do you expect out from ...',
    date: 'May 12, 2016'
  },
  {
    id: 4,
    title: 'Transcreation Gaining Momentum in the Translation Industry',
    category: 'Translation',
    excerpt: 'Transcreation is a process of adapting a creative piece of work into another language whilst maintaining its cultural impact ...',
    date: 'August 10, 2023'
  },
  {
    id: 5,
    title: 'Pay Attention to Your Packaging with Multilingual DTP',
    category: 'Interpretation, Transcription, Translation',
    excerpt: 'DTP stands for desktop publishing, which is a combination of personal computer and page layout software to create publication documents ...',
    date: 'June 10, 2016'
  },
  {
    id: 6,
    title: 'E-Learning Translation - Your Road to Cross-Cultural Adaptation',
    category: 'Translation',
    excerpt: 'E-learning translation is the perfect solution for today’s business needs because it helps firms offer coaching and re-coaching ...',
    date: 'April 10, 2016'
  },
  {
    id: 7,
    title: "Are You Outsourcing Multilingual DTP for Your Business?",
    category: "Interpretation, Transcription, Translation",
    excerpt: "This is something incredible you can try, that is outsourcing multilingual DTP if you are not doing it currently."
  },
  {
    id: 8,
    title: "CAT (Computer Assisted Translation) Which One Should You Be Using?",
    category: "Translation",
    excerpt: "Translation is converting a text or an article from one language to another language without changing the idea."
  },
  {
    id: 9,
    title: "Services in Pharmaceutical Industry/Healthcare/Medical Field",
    category: "Translation",
    excerpt: "Today, the global economy is dominated by English language. Yet there are many parts of the nation where language can be a barrier."
  },
  {
    id: 10,
    title: "Website Translation: Your Key to Global SEO",
    category: "Translation",
    excerpt: "Translation is one of the most important jobs in the world. Today, the world is becoming one through information and communication."
  },
  {
    id: 11,
    title: "Translation of Some of the Rare Indian Languages at Your Finger Tips",
    category: "Translation",
    excerpt: "Apart from common Indian languages such as Hindi, Bengali, Marathi, Punjabi, etc., sometimes you also come across various other rare languages."
  },
  {
    id: 12,
    title: "Eradicate the Challenges with Indian Languages",
    category: "Interpretation, Transcription, Translation",
    excerpt: "A modern way of capturing languages and translating has become really popular. Today, various tools and techniques are available to overcome language challenges."
  },
])

const searchTerm = ref('')
const currentPage = ref(1)
const postsPerPage = 9

const filteredPosts = computed(() => {
  if (!searchTerm.value) return posts.value
  return posts.value.filter(post =>
      post.title.toLowerCase().includes(searchTerm.value.toLowerCase())
  )
})

const totalPages = computed(() => {
  return Math.ceil(filteredPosts.value.length / postsPerPage)
})

const pagedPosts = computed(() => {
  const start = (currentPage.value - 1) * postsPerPage
  return filteredPosts.value.slice(start, start + postsPerPage)
})

const recentPosts = computed(() => {
  return posts.value.slice(0, 5)
})

const router = useRouter()

function goToPage(page) {
  currentPage.value = page
}

function prevPage() {
  if (currentPage.value > 1) currentPage.value--
}

function nextPage() {
  if (currentPage.value < totalPages.value) currentPage.value++
}

function goToPost(id) {
  // Replace with actual routing to blog post details
  alert(`Go to post id: ${id}`)
}
</script>

<style>
/* Optional: truncate long excerpts with line clamp */
.line-clamp-3 {
  display: -webkit-box;
  -webkit-line-clamp: 3;
  -webkit-box-orient: vertical;
  overflow: hidden;
}
.underline-careers {
  position: relative;
  display: inline-block;
}

.underline-careers::after {
  content: '';
  display: block;
  width: 50%;  /* Adjust the width of the underline */
  height: 3px;  /* Height of the blue line */
  background-color: #3498db;  /* Blue color */
  margin: 10px auto 0;  /* Centers the underline and adds some spacing */
}
.flex.justify-center.space-x-4.mt-12.mb-16 {
  padding-bottom: 10px;
}
</style>
