<template>
  <fixedheader/>
  <div class="min-h-screen bg-gray-50">
    <!-- Hero Section -->
    <div class="relative h-48 bg-cover bg-center py-35" :style="{ backgroundImage: 'url(/audio1.jpg)' }">

      <!-- Overlay -->
      <div class="absolute inset-0 bg-black opacity-50 z-0"></div> <!-- Overlay with black color and opacity -->

      <!-- Content -->
      <div class="relative z-10 flex items-center justify-center h-full">
        <h1 class="text-4xl md:text-5xl font-bold text-white text-center tracking-wide">
          AUDIO VISUAL SERVICES
        </h1>
      </div>
    </div>

    <!-- Main Content -->
    <div class="max-w-7xl mx-auto px-4 py-8">
      <div class="grid grid-cols-1 lg:grid-cols-4 gap-8">
        <!-- Sidebar Navigation -->
        <div class="lg:col-span-1">
          <nav class="rounded-lg p-6">
            <ul class="space-y-3">
              <li><a href="#" class="text-blue-600 hover:text-blue-800 text-sm">Data Capture Services</a></li>
              <li><a href="#" class="text-blue-600 hover:text-blue-800 text-sm">Translation Services</a></li>
              <li><a href="#" class="text-blue-600 hover:text-blue-800 text-sm">Transcription Services</a></li>
              <li><a href="#" class="text-blue-600 hover:text-blue-800 text-sm">Interpreting Services</a></li>
              <li class="font-semibold text-gray-800 text-sm">Audio Visual Services</li>
              <li class="ml-4"><a href="#" class="text-blue-600 hover:text-blue-800 text-sm">Multilingual Desktop Publishing</a></li>
              <li class="ml-4"><a href="#" class="text-blue-600 hover:text-blue-800 text-sm">Subtitling</a></li>
              <li class="ml-4"><a href="#" class="text-blue-600 hover:text-blue-800 text-sm">Voiceover</a></li>
              <li><a href="#" class="text-blue-600 hover:text-blue-800 text-sm">Languages we Translate</a></li>
              <li><a href="#" class="text-blue-600 hover:text-blue-800 text-sm">Multiple Language Translation</a></li>
              <li><a href="#" class="text-blue-600 hover:text-blue-800 text-sm">FAQs: Frequently Asked Questions</a></li>
            </ul>
          </nav>
        </div>

        <!-- Main Content Area -->
        <div class="lg:col-span-3">
          <div class="rounded-lg p-8">
            <div class="prose max-w-none">
              <p class="text-gray-600 mb-6">
                Apart from providing Voice Over and Subtitles for your projects or documentaries on screen, Coral Knowledge Services
                is also known for providing state of the art Audio Visual Services (AVS) to our clients.
              </p>

              <p class="text-gray-600 mb-6">
                We believe in delivering turn-key solutions. We help to convert your project or presentation to a wider number of
                clients. Our expert team of linguists, audio and re-write your projects according to your requirements and beautifies your
                presentations.
              </p>

              <p class="text-gray-600 mb-6 font-semibold">We achieve this by</p>

              <div class="space-y-6">
                <div>
                  <h3 class="font-semibold text-gray-800 mb-2">Extensive video debriefing:</h3>
                  <p class="text-gray-600 text-sm">
                    We use state-of-the-art software in order to decorate your videos and presentations. We
                    ensure that your video is precise, crisp, and as per the requirements of your viewers. We do this in our advanced
                    editing studios with the help of our experienced advisors.
                  </p>
                </div>

                <div>
                  <h3 class="font-semibold text-gray-800 mb-2">Providing high-quality voiceovers:</h3>
                  <p class="text-gray-600 text-sm">
                    At Coral Knowledge Services, we have the experience and the talent needed to
                    produce high-quality voice productions that deliver your video exactly the way you want it to be delivered. Providing
                    outstanding quality at competitive pricing with excellent customer service is our motto. We provide all types of
                    voice over services like Narrations, Voice prompts as well as Interactive Voice Response (IVR).
                  </p>
                </div>

                <div>
                  <h3 class="font-semibold text-gray-800 mb-2">Motion graphics and capture:</h3>
                  <p class="text-gray-600 text-sm">
                    The slick, network-quality imagery that was once affordable only to the major players
                    in advertising and marketing is now an affordable art form for virtually any company or business seeking to look as
                    good. Our clientele includes everyone from advertising companies to major corporate companies and hospitals. Our
                    motion graphics services also include the following:
                  </p>
                  <ul class="list-disc list-inside mt-2 text-gray-600 text-sm space-y-1">
                    <li>Digital Signage</li>
                    <li>Television programming</li>
                    <li>Websites</li>
                    <li>Video presentations</li>
                  </ul>
                </div>

                <div>
                  <h3 class="font-semibold text-gray-800 mb-2">Sound designing and re-production:</h3>
                  <p class="text-gray-600 text-sm">
                    Coral Knowledge Services wants your media production project to sound as
                    good as it looks and we have the tools and the talent to do just that. Our sound design and digital audio production
                    studio utilize the finest digital audio production facilities available, staffed by producers and technicians with an ear
                    for great audio. Audio for video and film, audio for web, podcasts, sound-sweetening, foreign-language audio, radio
                    commercials, special effect/special event audios, and custom jingle composition and production packages are all
                    available in one place. Our services include:
                  </p>
                  <ul class="list-disc list-inside mt-2 text-gray-600 text-sm space-y-1">
                    <li>Mixing</li>
                    <li>Mastering</li>
                    <li>Recording and Re-recording</li>
                    <li>Sound Designing</li>
                    <li>Engineering and others</li>
                  </ul>
                </div>
              </div>

              <div class="mt-8 pt-6 border-t border-gray-200">
                <h3 class="font-semibold text-gray-800 mb-2">Confidentiality</h3>
                <p class="text-gray-600 text-sm">
                  At Coral Knowledge Services we follow a principle of confidentiality and extreme secrecy with our clients.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
  <Footer/>
</template>

<script setup>
</script>

<style scoped>
.prose {
  color: inherit;
}
</style>
