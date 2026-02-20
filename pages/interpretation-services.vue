<template>
  <fixedheader/>
  <section class="w-full">
    <!-- Header with background image -->
    <div
        class="relative bg-cover bg-center bg-no-repeat py-30"
        style="background-image: url('/slide5.jpg')"
    >
      <!-- Dark overlay for better text readability -->
      <div class="absolute inset-0 bg-black opacity-50 z-0"></div> <!-- Changed to black overlay with opacity -->

      <div class="relative z-10 max-w-6xl mx-auto text-center">
        <h1 class="text-4xl md:text-5xl font-bold text-white mb-4">
    <span class="relative inline-block">
      INTERPRETING SERVICES
      <!-- Blue Underline under the text -->
      <div class="absolute bottom-0 left-0 w-full h-0.5 bg-blue-500"></div>
    </span>
        </h1>

      </div>

    </div>

    <!-- Content section -->
    <section class="bg-white py-16 px-4">
      <div class="max-w-6xl mx-auto">
        <div class="grid md:grid-cols-3 gap-12">

          <!-- Left Column - Services List -->
          <div class="space-y-6 px-8">
            <h2 class="text-2xl font-semibold text-gray-800 mb-6">Our Services</h2>
            <ul class="space-y-4">
              <li class="text-gray-600 hover:text-blue-600 transition-colors cursor-pointer font-medium">Data Capture Services</li>
              <li class="text-gray-600 hover:text-blue-600 transition-colors cursor-pointer font-medium">Translation Services</li>
              <li class="text-gray-600 hover:text-blue-600 transition-colors cursor-pointer font-medium">Transcription Services</li>
              <li class="text-gray-600 hover:text-blue-600 transition-colors cursor-pointer font-medium">Interpreting Services</li>
              <li class="text-blue-600 hover:text-blue-800 transition-colors cursor-pointer ml-4 font-medium">Legal Interpretation</li>
              <li class="text-blue-600 hover:text-blue-800 transition-colors cursor-pointer ml-4 font-medium">Medical Interpretation</li>
              <li class="text-gray-600 hover:text-blue-600 transition-colors cursor-pointer font-medium">Audio Visual Services</li>
              <li class="text-gray-600 hover:text-blue-600 transition-colors cursor-pointer font-medium">Languages we Translate</li>
              <li class="text-gray-600 hover:text-blue-600 transition-colors cursor-pointer font-medium">Multiple Language Translation</li>
              <li class="text-gray-600 hover:text-blue-600 transition-colors cursor-pointer font-medium">FAQs (Frequently Asked Questions)</li>
            </ul>
          </div>

          <!-- Right Column - Content -->
          <div class="col-span-2 space-y-8">
            <h3 class="text-2xl font-semibold text-gray-800 mb-4">About Our Services</h3>
            <p class="text-gray-700 leading-relaxed mb-6">
              Over the years, we have provided the best form of text interpretation and telephonic interpretations at ease and at
              affordable prices. Our interpretation services get your message across to a broader audience, expand the horizons of
              your possibilities, and comprehend what others offer.
            </p>

            <p class="text-gray-700 leading-relaxed mb-6">
              Coral Knowledge Solutions specializes in a full range of high-quality language interpretation services, from the
              translation of a one-page birth certificate to the coordination of multi-language, multi-venue simultaneous
              interpretation services for international conferences with thousands of international delegates.
            </p>

            <p class="text-gray-700 leading-relaxed mb-6">
              There are many reasons to communicate your message clearly and accurately, and when languages create a barrier,
              we can help you achieve your objectives efficiently and in a cost-effective manner with our interpretation services.
              Whether you need to understand or be understood in Spanish, Russian, Italian, French, Chinese, Korean, or Hebrew,
              you need a skilled interpreter and/or translator to get the job done and to give you a competitive edge. Coral
              Knowledge Services is committed to providing superior interpreting services to associations, corporations, individuals
              and any government office.
            </p>

            <p class="text-gray-700 leading-relaxed mb-6">
              Our simultaneous interpretation services allow you to have your message heard at conferences, meetings, international
              seminars, and other venues. Our simultaneous interpreters are skilled and experienced in listening to a message
              delivered in one language and interpreting the message in real-time, making international communication possible in
              any setting. Our conference interpreters work in pairs using highly advanced simultaneous interpretation equipment to
              ensure the success of your event.
            </p>

            <div class="mt-8">
              <h3 class="text-lg font-semibold text-gray-800 mb-4">Simultaneous Interpretation:</h3>
              <p class="text-gray-700 leading-relaxed mb-6">
                In order to think from to speak, but then, coordinating between the two poses a problem. That's where we come in.
                Our team of linguists helps to interpret your dialects personally whenever and wherever you need them. We specialize
                in simultaneous and immediate interpreting. This modality of interpretation generally requires the use of equipment,
                thus enabling transmission to audiences, large or small. For the most part, our skilled simultaneous interpreters work in
                pairs, in order to maintain the concentration required to perform the task at hand.
              </p>

              <h3 class="text-lg font-semibold text-gray-800 mb-4">Our Features:</h3>
              <ul class="space-y-4">
                <li class="flex items-start">
                  <span class="text-blue-600 mr-2">•</span>
                  <div>
                    <strong class="text-gray-800">Professional Work:</strong>
                    <span class="text-gray-700"> Our brilliant interpreters usually work in pairs and use the best available technology to provide accurate interpretations and flawless service.</span>
                  </div>
                </li>
                <li class="flex items-start">
                  <span class="text-blue-600 mr-2">•</span>
                  <div>
                    <strong class="text-gray-800">No Interruptions:</strong>
                    <span class="text-gray-700"> We use state-of-the-art equipment, for uninterrupted interpretations. Both the listener and speaker feel as if they're talking directly to one another.</span>
                  </div>
                </li>
                <li class="flex items-start">
                  <span class="text-blue-600 mr-2">•</span>
                  <div>
                    <strong class="text-gray-800">Effectiveness:</strong>
                    <span class="text-gray-700"> Our perfect services ensure efficient use of time. We install the equipment in advance and the interpreters are prepared ahead of time, to provide an excellent service.</span>
                  </div>
                </li>
                <li class="flex items-start">
                  <span class="text-blue-600 mr-2">•</span>
                  <div>
                    <strong class="text-gray-800">Multi-Language Interpretation:</strong>
                    <span class="text-gray-700"> We can interpret in not just one but several languages at affordable costs.</span>
                  </div>
                </li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </section>
  </section>

  <Footer/>
</template>

<script setup>
// Component for Interpreting Services section
</script>
