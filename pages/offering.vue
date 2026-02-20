<script setup lang="ts">
</script>
<template>
  <fixedheader/>
  <div class="min-h-screen offering-page">
    <!-- Hero Section -->
    <section
        class="relative flex items-center justify-center h-[30vh] text-white text-center bg-cover bg-center bg-no-repeat"
        style="background-image: url('/Contact-Us-1.jpg')"
    >
      <!-- Overlay -->
      <div class="absolute inset-0 bg-[#34495e] opacity-75"></div>

      <!-- Content -->
      <div class="relative max-w-3xl px-5">
        <h1 class="relative inline-block text-4xl md:text-5xl font-bold mb-8 tracking-[3px] uppercase">
          OFFERING
          <!-- Blue Underline under the text -->
          <div class="w-full h-[3px] bg-blue-500 mt-2 mx-auto"></div>
        </h1>

        <p class="max-w-xl mx-auto text-sm md:text-base leading-relaxed font-light opacity-90">
          IT IS BETTER TO HAVE READ A GREAT WORK OF ANOTHER CULTURE IN TRANSLATION THAN NEVER TO
          HAVE READ IT AT ALL
        </p>
      </div>
    </section>

    <!-- Main Content Section -->
    <section class="py-16 md:py-20 bg-gray-100">
      <div class="max-w-6xl mx-auto px-5">
        <!-- Intro -->
        <div class="mb-16 space-y-6">
          <p class="text-base leading-7 text-gray-600 text-justify">
            At Coral Knowledge Services, you will find a broad range of accurate translation and other related services. In today's dynamic world, it has become imperative to have, that is to say, a presence in different countries. However, to reach out to people in other countries, it is necessary that you communicate with people in the language that they understand. Thus, it becomes important to translate your key information, such as legal documents, financial documents, marketing communication, and all other business-critical information into other foreign languages.
          </p>
          <p class="text-base leading-7 text-gray-600 text-justify">
            We also address the need for other services such as interpretation, subtitling/captioning, voiceovers, and transcription in foreign languages. Apart from meeting the translation needs of businesses, we also serve individuals who are in need of translation services.
          </p>
        </div>

        <!-- Services List -->
        <div class="space-y-12">
          <!-- Translation Services -->
          <div>
            <h3 class="text-lg font-bold text-gray-800 tracking-wide  border-blue-500 inline-block pb-1 mb-4">
              TRANSLATION SERVICES
            </h3>
            <p class="text-base leading-7 text-gray-600 mb-2 text-justify">
              Coral Knowledge Services offers professional translation and proofreading services for a large variety of clients. While most of our customers are large businesses, we often get requests from individuals or smaller ventures and we gladly accept the same. Our main services consist of translation and proofreading and we have several years of experience in these subjects. We only employ native translators with proven experience that can live up to the high-quality standards of our company. Our translation services can help you mitigate the risks associated with venturing into another country, the native language of which you do not know.
            </p>
            <NuxtLink to="/translation-services" class="text-blue-600 font-semibold text-sm hover:underline">
              Read more
            </NuxtLink>
          </div>

          <!-- Transcription Services -->
          <div>
            <h3 class="text-lg font-bold text-gray-800 tracking-wide  border-blue-500 inline-block pb-1 mb-4">
              TRANSCRIPTION SERVICES
            </h3>
            <p class="text-base leading-7 text-gray-600 mb-2 text-justify">
              Coral Knowledge Services offers transcription services in different areas such as Legal, Medical, Insurance, Entertainment, Corporate, Government, and Education sectors. We provide accurate and on-time transcription services. Just one simple step, upload your audio/video files into our server and we will do the rest.
            </p>
            <NuxtLink to="/transcription-services" class="text-blue-600 font-semibold text-sm hover:underline">
              Read more
            </NuxtLink>
          </div>

          <!-- Interpretation Services -->
          <div>
            <h3 class="text-lg font-bold text-gray-800 tracking-wide  border-blue-500 inline-block pb-1 mb-4">
              INTERPRETATION SERVICES
            </h3>
            <p class="text-base leading-7 text-gray-600 mb-2 text-justify">
              Coral Knowledge Services offers immediate on-demand access to interpreters over the telephone in more than 200+ languages 24/7/365.
            </p>
            <p class="text-base leading-7 text-gray-600 mb-2 text-justify">
              Calls in any language across different time zones pose no problem. We have been handling these types of calls for over five years from large and small customers, from government agencies and private companies, medical facilities and insurance carriers, 911 operators, and emergency room staff.
            </p>
            <NuxtLink to="/interpretation-services" class="text-blue-600 font-semibold text-sm hover:underline">
              Read more
            </NuxtLink>
          </div>

          <!-- Audio Visual Services -->
          <div>
            <h3 class="text-lg font-bold text-gray-800 tracking-wide  border-blue-500 inline-block pb-1 mb-4">
              AUDIO VISUAL SERVICES
            </h3>
            <p class="text-base leading-7 text-gray-600 mb-2 text-justify">
              Coral Knowledge Services provides audio-visual services such as subtitling/captioning and voiceover services in different international and Indian languages in order to break language barriers and reach out to a large non-English populace. We have a team of language professionals who are experienced in providing audio-visual services such as subtitling and voiceovers in different languages. Having expertise in over 35 languages (the list is increasing), we are capable of providing audio-visual services in various languages, dialects, and accents.
            </p>
            <NuxtLink to="/audio-visual-services" class="text-blue-600 font-semibold text-sm hover:underline">
              Read more
            </NuxtLink>

          </div>

          <!-- Data Capture Services -->
          <div>
            <h3 class="text-lg font-bold text-gray-800 tracking-wide border-blue-500 inline-block pb-1 mb-4">
              DATA CAPTURE SERVICES
            </h3>
            <p class="text-base leading-7 text-gray-600 mb-2 text-justify">
              From manual punching of data to automated capturing, Coral Knowledge Services offers services specifically tailored to meet all your data-capturing requirements. Also, we focus relentlessly to provide our clients with high-quality data-capturing services cost-effectively and within due time.
            </p>
            <NuxtLink to="/data-capture-services" class="text-blue-600 font-semibold text-sm hover:underline">
              Read more
            </NuxtLink>
          </div>
        </div>
      </div>
    </section>
  </div>
  <Footer/>
</template>

<style scoped>
p.max-w-xl.mx-auto.text-sm.md\:text-base.leading-relaxed.font-light.opacity-90 {
  color: #fff;
}
</style>