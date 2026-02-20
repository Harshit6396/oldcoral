<template>
  <section class="py-16 px-4 max-w-7xl mx-auto">
    <div class="text-center mb-16">
      <h2 class="text-2xl font-semibold text-gray-700 tracking-wide">OUR EXPERTISE</h2>
    </div>

    <div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-12 lg:gap-16">
      <div v-for="(item, index) in expertiseData" :key="index" class="flex items-start gap-6">
        <!-- Updated to use direct Unicode characters instead of Font Awesome classes -->
        <div class="icon-container w-16 h-16 bg-yellow-400 rounded-full flex items-center justify-center flex-shrink-0">
          <span class="icon-symbol text-white text-2xl font-bold">{{ item.iconSymbol }}</span>
        </div>

        <div class="flex-1">
          <h3 class="text-gray-700 font-semibold text-sm tracking-wide mb-4 leading-tight">{{ item.title }}</h3>
          <p class="text-gray-600 text-sm leading-relaxed">{{ item.description }}</p>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const expertiseData = [
  {
    iconSymbol: "🖥️",
    title: "WEBSITE TRANSLATION",
    description:
        "We can help your business achieve greater customer reach. We will not only provide you with a 100% accurate translation of the original text but also adapt your website content to the targeted market.",
  },
  {
    iconSymbol: "⚙️",
    title: "TECHNICAL TRANSLATION SERVICES",
    description:
        "When translating technical documents it's essential that all the terminology is translated correctly. Taken to an extreme, technical translation can literally be the difference between life and death.",
  },
  {
    iconSymbol: "📈",
    title: "MARKETING TRANSLATIONS SERVICES",
    description:
        "Marketing Translations are Crucial. When you have spent countless hours getting your brand message right, why then choose translation services that destroy your message in other languages?",
  },
  {
    iconSymbol: "📄",
    title: "BUSINESS TRANSLATION SERVICE",
    description:
        "We understand the needs of your business. What you get with us is nothing less than top quality translation services for all your business related documents.",
  },
  {
    iconSymbol: "⚖️",
    title: "LEGAL INTERPRETATION",
    description:
        "Our court interpreters have years of courtroom translating experience. They understand foreign cultures and business etiquette — valuable skills for face-to-face interpreting. And you can rely on us for complete confidentiality.",
  },
  {
    iconSymbol: "🏥",
    title: "MEDICAL TRANSCRIPTION",
    description:
        "We are truly a one-stop solution for all your medical transcription needs and have become the preferred choice of our healthcare providers for their medical transcription needs.",
  },
]
</script>

<!-- Removed Font Awesome CSS since we're using Unicode symbols -->
<style scoped>
.icon-container {
  position: relative;
}

.icon-symbol {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 100%;
  height: 100%;
  color: white; /* Ensures icon symbols are white */
}
</style>
