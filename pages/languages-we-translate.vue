<template>
  <fixedheader/>
  <div class="min-h-screen">
    <!-- Hero Section with Background -->
    <section
        class="relative h-64 flex items-center justify-center bg-cover bg-center bg-no-repeat"
        :style="{ backgroundImage: 'url(/company.png)' }"
    >
      <!-- Dark overlay -->
      <div class="absolute inset-0 bg-black opacity-50 z-0"></div>

      <!-- Content -->
      <h1 class="relative text-white text-4xl font-bold tracking-wider z-10">
  <span class="relative inline-block">
    LANGUAGES WE TRANSLATE
    <!-- Blue Underline under the text -->
    <div class="absolute bottom-0 left-0 w-full h-0.5 bg-blue-500"></div>
  </span>
      </h1>

    </section>


    <!-- Main Content -->
    <div class="container mx-auto px-4 py-12">
      <div class="grid grid-cols-1 lg:grid-cols-4 gap-8">
        <!-- Sidebar Navigation -->
        <aside class="lg:col-span-1">
          <nav class="space-y-2">
            <NuxtLink
                v-for="service in services"
                :key="service.name"
                :to="service.link"
                class="block text-gray-600 hover:text-blue-600 py-2 border-b border-gray-200"
            >
              {{ service.name }}
            </NuxtLink>
          </nav>
        </aside>

        <!-- Main Content Area -->
        <main class="lg:col-span-3">
          <div class="prose max-w-none">
            <p class="text-gray-700 mb-6">
              Finding the right language translation service can pose a problem. At Coral Knowledge Services, we strive to help you navigate a multilingual world in order to overcome all your linguistic challenges. These may include major issues of language competency, technology, industry knowledge, delivery deadlines, and others that make this decision even harder. In a wide world of languages, you might be lost if not given the proper guidance.
            </p>

            <p class="text-gray-700 mb-8">
              We at Coral Knowledge Services translate from and to a plethora of languages. All languages are local to us. Here we employ the best personnel who not just speak but literally breathe the language. All our team members are native speakers of their language. They are screened through rigorous quality processes. We translate anything and everything. Over the years Coral Knowledge Services has been known far and wide for its outstanding quality. Not only do we translate but localize as well.
            </p>

            <h3 class="text-xl font-semibold mb-4">Some of the common languages include:</h3>

            <div class="space-y-6">
              <div v-for="language in languages" :key="language.name">
                <h4 class="font-semibold text-lg mb-2">{{ language.name }}</h4>
                <p class="text-gray-700">{{ language.description }}</p>
              </div>
            </div>
          </div>
        </main>
      </div>
    </div>
  </div>
  <Footer/>
</template>

<script setup>
// Services navigation data
const services = [
  { name: 'Data Capture Services', link: '/data-capture-services' },
  { name: 'Translation Services', link: '/translation-services' },
  { name: 'Transcription Services', link: '/transcription-services' },
  { name: 'Interpreting Services', link: '/interpreting-services' },
  { name: 'Audio Visual Services', link: '/audio-visual-services' },
  { name: 'Languages we Translate', link: '/languages-we-translate' },
  { name: 'Multiple Language Translation', link: '/multiple-language-translation' },
  { name: 'FAQs (Frequently Asked Questions)', link: '/faqs-frequently-asked-questions' }
]

// Language descriptions data
const languages = [
  {
    name: 'Arabic translation',
    description: 'Say "Ahla wa sahla" (goodbye) to your linguistic troubles after we say "marhaban" (hello) to you. Coral Knowledge Services can provide Arabic translations for a wide range of works, such as marketing materials, books, legal, medical, and technical documents, and much more, at a reasonable price to help you communicate with Arabic speakers. Our Arabic translators have excellent linguistic qualifications and years of experience in the Arabic translation service industry. They also have degrees in fields such as medicine, law, and engineering. Our highly trained Arabic dialect translators work on projects related to their subject matter expertise to assure the alternatives in the Arabic language are translated properly for a particular topic.'
  },
  {
    name: 'Chinese Translation',
    description: 'China is an economic powerhouse; it represents one-fifth of the world\'s population and markets, with almost over a billion Chinese speakers worldwide. This translates into a huge client base with economic, political, and cultural exchanges that require clear communications. Our highly-skilled translators are among the best in the Chinese translation service industry. All of our Chinese translations are thoroughly proofread by editors to make sure that the accurate meaning of the original content is kept intact. Moreover, we also undertake tedious quality tests in order to provide the content of your script as it is.'
  },
  {
    name: 'Dutch Translation',
    description: 'Hallo that\'s "hello" in Dutch world! At Coral Knowledge Services, we offer quality Dutch translation services. We translate all types of documents to and from Dutch at affordable rates. Our Dutch translation projects are accurately handled by the best translators in the industry.'
  },
  {
    name: 'Japanese translation',
    description: '"Konichi Wa!" We provide a variety of excellent, fast-paced, and timely services to translate all your business, legal, medical, technical, and other documents from and to Japanese.'
  }
]

// SEO Meta
useHead({
  title: 'Languages We Translate - Translation Services',
  meta: [
    { name: 'description', content: 'Professional translation services for multiple languages including Arabic, Chinese, Dutch, and Japanese.' }
  ]
})
</script>