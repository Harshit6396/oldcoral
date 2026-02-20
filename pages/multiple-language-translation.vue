<template>
  <fixedheader/>
  <div class="min-h-screen bg-gray-50">
    <!-- Hero Section with Background -->
    <section
        class="relative h-64 flex items-center justify-center bg-cover bg-center bg-no-repeat"
        :style="{ backgroundImage: 'url(/company.png)' }"
    >
      <!-- Overlay -->
      <div class="absolute inset-0 bg-black opacity-60 z-0"></div> <!-- Overlay with black color and opacity -->

      <!-- Content -->
      <h1 class="relative text-white text-4xl font-bold tracking-wider text-center px-4 z-10">
  <span class="relative inline-block">
    MULTIPLE LANGUAGE TRANSLATION
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
          <nav class="p-6">
            <ul class="space-y-3">
              <li v-for="service in services" :key="service.name">
                <NuxtLink
                    :to="service.link"
                    class="block text-gray-600 hover:text-blue-600 py-2 border-b border-gray-200"
                >
                  {{ service.name }}
                </NuxtLink>
              </li>
            </ul>
          </nav>
        </aside>

        <!-- Main Content Area -->
        <main class="lg:col-span-3">
          <div class=" p-8">
            <div class="prose max-w-none text-gray-700 leading-relaxed">
              <p class="mb-6">
                At Coral Knowledge Services we offer language services on a global scale to both individuals and businesses alike.
                In order to deliver accurate translations to our clients, we assure that at every stage in the translation process, we have
                serious quality checks built in. Our team comprises the best translators worldwide. Every language is local to us. We
                offer you to get rid of your language barriers. Our translators are seasoned professionals and highly experienced.
                Moreover, they have been screened efficiently to meet not only the industry's standards but also cater exactly and
                flawlessly to the needs of our clientele.
              </p>

              <p class="mb-6">
                Projects are finely translated into the required native language and will be assigned to an expert project manager
                and proven best expertise in the subject field and proven track record, relating to accuracy, speed, and overall
                performance.
              </p>

              <h3 class="text-lg font-semibold text-gray-800 mb-3">Why will you choose us?</h3>
              <p class="mb-6">
                Why not? We provide you with the best in the industry. Excellent team, top-class services. Wide client base, over-the-
                top expertise, vast experience. You name it we have it for you!
              </p>

              <p class="mb-6">And apart from that we have:</p>

              <div class="space-y-6">
                <div>
                  <h4 class="font-semibold text-gray-800 mb-2">Competitive Prices</h4>
                  <p>
                    It has been guaranteed by all our satisfied customers, that the prices quoted by us are the lowest in the industry.
                    Market surveys show that we are among those who charge the least worldwide.
                  </p>
                </div>

                <div>
                  <h4 class="font-semibold text-gray-800 mb-2">Millions of Major Languages worldwide</h4>
                  <p>
                    Yes, we can speak and understand every language in the world. Our management staff has painstakingly built a team
                    of knowledgeable and passionate language service professionals, devoted to taking care of your problems in
                    translation and providing the best solutions to you. Within the realm of ever-expanding global markets, we are ready to
                    help our valuable clients allowing them to meet their goals and objectives. Moreover, we stay back after our work is
                    completed asking you is any further arising post-translation. We form lasting relationships with educated, certified, and
                    affirmed linguists from respected universities and colleges around the world.
                  </p>
                </div>

                <div>
                  <h4 class="font-semibold text-gray-800 mb-2">All Specializations</h4>
                  <p>
                    All of our experts are not only qualified but are extremely talented as well. We at Coral Knowledge Services, believe not
                    only in just translating documents, but building long-lasting relations with clients. We have translated into many
                    languages like Hebrew, Chinese, Japanese, Dutch, Greek, French, Italian, and Spanish to name a few.
                  </p>
                </div>

                <div>
                  <h4 class="font-semibold text-gray-800 mb-2">Exceptional Customer Service</h4>
                  <p>
                    All our customers receive personalized service. That's what we believe in. We strive to complete your translations in
                    time. Moreover, we stay there to relieve you of any hassles post our task.
                  </p>
                </div>

                <div>
                  <h4 class="font-semibold text-gray-800 mb-2">Quality Assurance System</h4>
                  <p>
                    At Coral Knowledge Systems all our projects undergo rigorous scrutiny until our clients are satisfied. We are always on
                    the upgrade and use standardized quality screening methods to keep up with the industry levels.
                  </p>
                </div>

                <div>
                  <h4 class="font-semibold text-gray-800 mb-2">24/7 Technical Support</h4>
                  <p>We can work at any time frame provided by you.</p>
                </div>
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

// SEO Meta
useHead({
  title: 'Multiple Language Translation Services - Professional Translation',
  meta: [
    {
      name: 'description',
      content: 'Professional multiple language translation services with competitive prices, quality assurance, and 24/7 support. Expert translators for all major languages worldwide.'
    }
  ]
})
</script>