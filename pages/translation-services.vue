<template>
  <fixedheader/>
  <section class="w-full">
    <!-- Header Section -->
    <div class="bg-gradient-to-r from-slate-500 to-slate-600 py-30 px-4">
      <div class="max-w-6xl mx-auto text-center">
        <h1 class="text-4xl md:text-5xl font-bold text-white mb-4">
          <span class="relative inline-block">
            TRANSLATION SERVICES
            <!-- Underline under the text -->
            <div class="absolute bottom-0 left-0 w-full h-0.5 bg-blue-500"></div>
          </span>
        </h1>
      </div>
    </div>

    <!-- Content Section -->
    <div class="bg-white py-16 px-4">
      <div class="max-w-6xl mx-auto">
        <div class="grid md:grid-cols-2">
          <!-- Left Column - Services List -->
          <div class="space-y-4">
            <div class="text-center mb-8">
              <h2 class="text-lg font-semibold text-[#3170ac] mb-6">Data Capture Services</h2>
              <div class="space-y-3">
                <div v-for="service in services" :key="service.name" class="text-[#3170ac] hover:text-blue-800 cursor-pointer transition-colors">
                  <router-link :to="service.link">{{ service.name }}</router-link>
                </div>
              </div>
            </div>

            <div class="text-center">
              <h2 class="text-lg font-semibold text-[#3170ac] mb-6">Transcription Services</h2>
              <div class="space-y-3">
                <div v-for="transcription in transcriptionServices" :key="transcription.name" class="text-[#3170ac] hover:text-blue-800 cursor-pointer transition-colors">
                  <router-link :to="transcription.link">{{ transcription.name }}</router-link>
                </div>
              </div>
            </div>
          </div>

          <!-- Right Column - Content -->
          <div class="space-y-6 text-gray-700 leading-relaxed">
            <p>
              At Coral Knowledge Services, we translate and help translate from and to any language. As has been vouched for by our vast client base, we can boast that our services are 100% accurate. Not only do we translate, but we also edit and proofread documents as well. Our linguists are available worldwide providing our customers with the professional assistance in making their business available in every part of the world. We are conversant in every existing language and translate documents at low costs.
            </p>
            <p>
              Apart from translating the language, we also rephrase and/or reframe the document at an additional cost in order to meet the client's needs. We provide fast and effective translations of documents at reasonable prices. Moreover, we also help translate technical documents into a native language so as to help our customers. We have teamed up with translators all over the world and we have served various industries like Pharmaceutical, IT, Gaming industry, Automobile industry etc. Over the years, we have built a team with people who are enriched with wide experience and knowledge and we believe loyalty serves our needs.
            </p>
            <p>
              <strong>Quality:</strong> At Coral Knowledge Services, we have well-defined quality protocols, by which we abide in order to maintain our quality standards. We tend to hire the expertise that understands words, not merely know them. Moreover, every document is re-read and edited thoroughly to meet international standards. We use up-to-date software for fast and effective translation. We pledge to maintain extreme confidentiality while translating sensitive documents.
            </p>
            <p>
              <strong>Industries we cater to:</strong> Coral Knowledge Services caters to a vast array of industries like Pharmaceuticals, Hospitals, Biotech, IT, Media, Publishing, Gaming, Education, Telecommunication, Banking and Investments, Government Sectors, Science and Technology, Legal Services, Visa Translation, Translation of Certificates and other important documents. We translate various types of documents like brochures, manuals, product details, catalogs, CAD drawings, marketing materials, business proposals, and training materials.
            </p>
            <p>
              We also translate <strong>Medical Documents:</strong> Medical translation involves a long and tedious process to introduce a new drug into the market. It can be highly expensive and may delay the drug launch if not properly done. Over the years we have translated Clinical data, Medical information, and Quality manuals. Our association with doctors and other medical and para-medical practitioners has aided in our progress. We have translated a plethora of medical subjects worldwide.
            </p>
            <p>
              <strong>Languages known to us:</strong> As mentioned all the languages are local to us. We have done major translation works in Asian, Middle Eastern and European languages. Our languages include Dutch, Chinese, German, French, Hebrew, Russian, Korean, Vietnamese, Portuguese, Spanish, and Italian.
            </p>
          </div>
        </div>
      </div>
    </div>

  </section>
  <Footer />
</template>

<script setup>
// Service data with links to respective pages
const services = [
  { name: 'Translation Services', link: '/translation-services' },
  { name: 'Financial Translation', link: '/financial-translation-services' },
  { name: 'Legal Translation', link: '/legal-translation-services' },
  { name: 'Healthcare & Medical Translation', link: '/healthcaremedical-translation' },
  { name: 'Engineering & Technical Translation', link: '/engineering-technical-translation' },
  { name: 'Automotive Industries Translation', link: '/industry-automotive' },
  { name: 'What is Gaming Website Translation?', link: '/industry-gaming' },
  { name: 'E-learning and Training Material', link: '/industry-elearning' }
]

const transcriptionServices = [
  { name: 'Interpreting Services', link: '/interpreting-services' },
  { name: 'Audio Visual Services', link: '/audio-visual-services' },
  { name: 'Languages we Translate', link: '/languages-we-translate' },
  { name: 'Multiple Language Translation', link: '/multiple-language-translation' },
  { name: 'FAQs Frequently Asked Questions', link: '/faqs-frequently-asked-questions' }
]
</script>

<style scoped>
/* Additional custom styles if needed */
</style>