<template>
  <div class="min-h-screen bg-white">
    <!-- Header Navigation -->
    <fixedheader />

    <ImageSlider />

    <section class="bg-white py-16">
      <div class="container mx-auto px-4">
        <div class="grid md:grid-cols-3 gap-8 max-w-6xl mx-auto">
          <div class="text-center">
            <img
                src="/company.png"
                alt="Professional Meeting"
                class="w-full h-48 object-cover rounded-lg mb-4"
            />
            <h3 class="font-bold text-lg mb-2 border-b-2 border-blue-500 inline-block ">
              COMPANY
            </h3>
            <p class="text-gray-600 text-sm">
              Established in 2009, Coral is a premier provider of multilingual and multicultural communication solutions.
            </p>
          </div>

          <div class="text-center">
            <img
                src="/searvices.jpg"
                alt="Outdoor Discussion"
                class="w-full h-48 object-cover rounded-lg mb-4"
            />
            <h3 class="font-bold text-lg mb-2 border-b-2 border-blue-500 inline-block">
              SERVICES
            </h3>
            <p class="text-gray-600 text-sm">
              Coral Knowledge Services provides a full suite of linguistic services in all modern commercial languages, as well as languages of emerging Asian markets.
            </p>
          </div>

          <div class="text-center">
            <img
                src="/translation.jpg"
                alt="Professional Woman"
                class="w-full h-48 object-cover rounded-lg mb-4"
            />
            <h3 class="font-bold text-lg mb-2 border-b-2 border-blue-500 inline-block ">
              LANGUAGES
            </h3>
            <p class="text-gray-600 text-sm">
              One of Coral’s major focuses is on providing Indian language solutions for companies venturing into the new and potentially confusing world of emerging Asian markets.
            </p>
          </div>
        </div>
      </div>
    </section>


    <!-- Industries Section -->
    <section class="bg-gray-50 py-16">
      <div class="container mx-auto px-4">
        <div class="text-center text-[#2d2d2d] text-2xl mb-12">INDUSTRIES WE WORK FOR</div>
        <div class="grid md:grid-cols-4 gap-8 max-w-6xl mx-auto">
          <div>
            <h3 class="text-[#2d2d2d] mb-4 relative inline-block">
              FINANCIAL INDUSTRIES
              <!-- Full width border only under text -->
              <div class="absolute bottom-0 left-0 w-full border-b-2 border-blue-600"></div>
            </h3>
            <p class="text-gray-600 text-sm">
              Globalizing the Banking Industry with Custom Application Development as the banking industry continues to consolidate, institutions are seeking innovative, new ways to serve customers across regional and cultural boundaries.
            </p>
          </div>

          <div>
            <h3 class="text-[#2d2d2d] mb-4 relative inline-block">
              LEGAL INDUSTRIES
              <!-- Full width border only under text -->
              <div class="absolute bottom-0 left-0 w-full border-b-2 border-blue-600"></div>
            </h3>
            <p class="text-gray-600 text-sm">
              We provide specialist language solutions for the legal industry. Translations are available in all commercial languages and can be notarized for acceptance by any court or government agency in the United States or abroad.
            </p>
          </div>

          <div>
            <h3 class="text-[#2d2d2d] mb-4 relative inline-block">
              ENGINEERING & TECHNICAL
              <!-- Full width border only under text -->
              <div class="absolute bottom-0 left-0 w-full border-b-2 border-blue-600"></div>
            </h3>
            <p class="text-gray-600 text-sm">
              Our Engineering and Technical Translation solutions tailored to meet the needs of major contractors commissioned with large-size and extremely complex projects.
            </p>
          </div>

          <div>
            <h3 class="text-[#2d2d2d] mb-4 relative inline-block">
              AUTOMOTIVE & OTHERS
              <!-- Full width border only under text -->
              <div class="absolute bottom-0 left-0 w-full border-b-2 border-blue-600"></div>
            </h3>
            <p class="text-gray-600 text-sm">
              We are a leading translation provider to the automotive sector helping OEMs, suppliers and dealerships deploy solutions that turn translation into a competitive advantage.
            </p>
          </div>
        </div>
      </div>
    </section>

    <!-- Statistics Section -->
    <section
        class="relative bg-cover bg-center py-40"
        :style="{
    backgroundImage: 'linear-gradient(rgba(0,0,0,0.7), rgba(0,0,0,0.7)), url(\'https://i.ibb.co/j97fLjvj/blog21.jpg\')'
  }"
    >
      <div class="container mx-auto px-4">
        <h2 class="text-center text-white text-2xl font-bold mb-12">OUR AMAZING ACHIEVEMENTS</h2>
        <div class="grid md:grid-cols-4 gap-8 text-center text-white">
          <div>
            <div class="font-bold mb-2">
              <span class="text-4xl border-b-2 border-blue-600 w-20 inline-block">2009</span>
            </div>

            <div class="text-sm opacity-80">Company was established</div>
          </div>
          <div>
            <div class="font-bold mb-2">
              <span class="text-4xl border-b-2 border-blue-600 w-20 inline-block">79</span>
            </div>

            <div class="text-sm opacity-80">Expert linguist translators</div>
          </div>
          <div>
            <div class="font-bold mb-2">
              <span class="text-4xl border-b-2 border-blue-600 w-20 inline-block">72k</span>
            </div>

            <div class="text-sm opacity-80">Projects we have delivered</div>
          </div>
          <div>
            <div class="font-bold mb-2">
              <span class="text-4xl border-b-2 border-blue-600 w-20 inline-block">4000+</span>
            </div>

            <div class="text-sm opacity-80">Happy customers</div>
          </div>
        </div>
      </div>
    </section>

    <!-- Expertise Section -->
    <expertisesection />

    <!-- Get In Touch Section -->
    <getintouchsection />

    <Footer/>
  </div>

</template>

<script setup>


import Footer from "~/components/footer.vue";

useHead({
  title: 'KnowledgeTrans - Professional Translation Services',
  meta: [
    { name: 'description', content: 'Professional translation services worldwide in over 100 languages. Expert e-learning and localization engineering solutions.' }
  ]
})
</script>

<style scoped>
/* Additional custom styles if needed */
</style>
