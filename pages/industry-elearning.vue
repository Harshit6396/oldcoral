<template>
  <Fixedheader/>
  <!-- Header Section -->
  <section
      class="relative h-64 flex items-center justify-center bg-cover bg-center bg-no-repeat"
      :style="{ backgroundImage: 'url(/elearning.jpg)' }"
  >
    <!-- Dark Overlay -->
    <div class="absolute inset-0 bg-black opacity-50 z-0"></div>

    <!-- Text with Blue Underline -->
    <h1 class="relative text-white text-4xl font-bold tracking-wider z-10">
    <span class="relative inline-block">
      E-LEARNING AND TRAINING
      <!-- Blue Underline under the text -->
      <div class="absolute bottom-0 left-0 w-full h-0.5 bg-blue-500"></div>
    </span>
    </h1>
  </section>

  <div class="container mx-auto p-6 flex">

    <!-- Left Sidebar (Navigation) -->
    <div class="w-1/4  p-4">
      <ul class="space-y-4">
        <!-- Data Capture Services -->
        <li class="page_item">
          <a href="http://old.coralknowledgeservices.in/offering/data-capture-services/" class="text-lg text-blue-700 hover:underline">Data Capture Services</a>
        </li>
        <!-- Translation Services with Submenu -->
        <li class="page_item has_children">
          <a href="http://old.coralknowledgeservices.in/offering/translation-services/" class="text-lg text-black-700 hover:underline">Translation Services</a>
          <ul class="grandchild-sidebar-menu level-1 children pl-4">
            <li class="page_item">
              <a href="http://old.coralknowledgeservices.in/offering/translation-services/business-translation/" class="text-lg text-blue-600 hover:underline">Business Translation</a>
            </li>
            <li class="page_item ">
              <a href="http://old.coralknowledgeservices.in/offering/translation-services/financial-translation-services/" class="text-lg text-blue-600 hover:underline">Financial Translation</a>
            </li>
            <li class="page_item">
              <a href="http://old.coralknowledgeservices.in/offering/translation-services/technical-translation-services/" class="text-lg text-blue-600 hover:underline">Technical Translation</a>
            </li>
            <li class="page_item">
              <a href="http://old.coralknowledgeservices.in/offering/translation-services/document-translation-services/" class="text-lg text-blue-600 hover:underline">Document Translation</a>
            </li>
            <li class="page_item">
              <a href="http://old.coralknowledgeservices.in/offering/translation-services/visa-translation-services/" class="text-lg text-blue-600 hover:underline">Certified Visa Translation</a>
            </li>
            <li class="page_item ">
              <a href="http://old.coralknowledgeservices.in/offering/translation-services/legal-translation-services/" class="text-lg text-blue-600 hover:underline">Legal Translation</a>
            </li>
            <li class="page_item">
              <a href="http://old.coralknowledgeservices.in/offering/translation-services/medical-translation-services/" class="text-lg text-blue-600 hover:underline">Medical Translation</a>
            </li>
            <li class="page_item">
              <a href="http://old.coralknowledgeservices.in/offering/translation-services/website-translation-services/" class="text-lg text-blue-600 hover:underline">Website Localisation Service</a>
            </li>
            <li class="page_item">
              <a href="http://old.coralknowledgeservices.in/offering/translation-services/certified-translation/" class="text-lg text-blue-600 hover:underline">Certified Translation</a>
            </li>
            <li class="page_item">
              <a href="http://old.coralknowledgeservices.in/offering/translation-services/marketing-translation/" class="text-lg text-blue-600 hover:underline">Marketing Translation</a>
            </li>
            <li class="page_item">
              <a href="http://old.coralknowledgeservices.in/offering/translation-services/market-research-translation/" class="text-lg text-blue-600 hover:underline">Market Research Translation</a>
            </li>
            <li class="page_item">
              <a href="http://old.coralknowledgeservices.in/offering/translation-services/healthcaremedical-translation/" class="text-lg text-blue-600 hover:underline">Healthcare &amp; Medical Translation</a>
            </li>
            <li class="page_item " >
              <a href="http://old.coralknowledgeservices.in/offering/translation-services/engineering-technical-translation/" class="text-lg text-blue-600 hover:underline">Engineering &amp; Technical Translation</a>
            </li>
            <li class="page_item">
              <a href="http://old.coralknowledgeservices.in/offering/translation-services/industry-automotive/" class="text-lg text-blue-600 hover:underline">Automotive Industries Translation</a>
            </li>
            <li class="page_item">
              <a href="http://old.coralknowledgeservices.in/offering/translation-services/industry-gaming/" class="text-lg text-blue-600 hover:underline">What is Gaming Website Translation?</a>
            </li>
            <li class="page_item current_page_item">
              <a href="http://old.coralknowledgeservices.in/offering/translation-services/industry-elearning/" class="text-lg text-blue-600 hover:underline">E- learning and Training Material</a>
            </li>
          </ul>
        </li>

        <!-- Other Menu Items -->
        <li class="page_item">
          <a href="http://old.coralknowledgeservices.in/offering/transcription-services/" class="text-lg text-blue-700 hover:underline">Transcription Services</a>
        </li>
        <li class="page_item">
          <a href="http://old.coralknowledgeservices.in/offering/interpretation-services/" class="text-lg text-blue-700 hover:underline">Interpreting Services</a>
        </li>
        <li class="page_item">
          <a href="http://old.coralknowledgeservices.in/offering/audio-visual-services/" class="text-lg text-blue-700 hover:underline">Audio Visual Services</a>
        </li>
        <li class="page_item">
          <a href="http://old.coralknowledgeservices.in/offering/languages-we-translate/" class="text-lg text-blue-700 hover:underline">Languages we Translate</a>
        </li>
        <li class="page_item">
          <a href="http://old.coralknowledgeservices.in/offering/multiple-language-translation/" class="text-lg text-blue-700 hover:underline">Multiple Language Translation</a>
        </li>
        <li class="page_item">
          <a href="http://old.coralknowledgeservices.in/offering/faqs-frequently-asked-questions/" class="text-lg text-blue-700 hover:underline">FAQ’s (Frequently Asked Questions)</a>
        </li>
      </ul>
    </div>

    <!-- Right Content Section -->
    <div class="w-3/4 p-6">
      <!-- Header Section -->

      <!-- What is it Section -->
      <section id="whats-it" class="mb-12">
        <p>Just like sales and marketing, education, learning, and training are vital components of any business, no matter how big or how small. Apart from training new employees, there is a constant need to ensure associates are up-to-date on the latest technology, product improvement, customer service, and more. For international companies, there is a constant challenge to provide all of the employees with the same training courses and related materials wherever they are in the world and no matter what language they speak. We say, “Let the eLearning and translation experts at Coral Knowledge Services help.” Whether you represent an educational or training facility, a large company or a small business, Coral Knowledge Services can help you create a diverse and appealing multilingual eLearning or training solution that meets your clients’ specific needs.</p>
      </section>

      <!-- Our Services Section -->
      <section id="our-services" class="mb-12">
        <h2 class="text-2xl font-semibold text-gray-800">Innovative and Highly Effective Global eLearning Solutions</h2>
        <p>At Coral Knowledge Services, we understand that one should use not just effective but also innovative and creative eLearning and training programs that spark interest, and appeal to your audience apart from delivering the best results – all within an affordable budget. Moreover, for multinational organizations with a wide client base, it is necessary to ensure that all elements of your program are precisely and correctly translated and localized for your desired audience. If the language and context are not genuine and appropriate, it would turn out to be a waste of your time and money.</p><br>
        <p>Our experts work hard to create accurate eLearning solutions for all sorts of businesses. We develop everything from communicational aids to online quizzes to enhance your website. Coral Knowledge Services can help you design creative eLearning and teaching software in various languages to meet your specific goals. Our eLearning and translation professionals possess the expertise to develop consistent, high-quality instructional content for comprehensive learning programs in over a million languages.</p>
      </section>

      <!-- Documents We Translate Section -->
      <section id="documents" class="mb-12">
        <h3 class="text-xl font-semibold text-gray-800">Apart from Translation and Localization of Content, Our Comprehensive eLearning Services Include:</h3>
        <ul class="list-disc pl-6">
          <li>Multilingual manual design consultation</li>
          <li>Conversion of former training materials into an eLearning format</li>
          <li>Localization of software applications, web applications, and documentation</li>
          <li>Development of multilingual presentations like texts, audio and video content, as well as voiceover for radio and television</li>
          <li>Narrowing down of multimedia and marketing materials to specific languages</li>
          <li>Quality testing of the final product to ensure an accurate and appropriate adaptation of your materials</li>
        </ul>
      </section>

      <!-- Our Workflow Section -->
      <section id="workflow" class="mb-12">
        <h3 class="text-xl font-semibold text-gray-800">Optimizing Your Multilingual eLearning Capabilities</h3>
        <p>Coral Knowledge Services can help you optimize your multilingual eLearning capabilities and effectively reach your global target audiences.</p><br>
        <p><strong>Speak to us today!</strong> For more information on how CORAL can assist you with your translation and eLearning requirements, please contact us through this website, or call us at +91-981-868-1169 in Asia.</p>
      </section>
    </div>


  </div>
  <Footer/>
</template>

<script>
export default {
  name: "FinancialTranslationPage",
};
</script>

<style scoped>
/* Sidebar and Content Styling */
.page_item a {
  display: block;
  padding: 1px 12px;
  font-size: 1rem;
  color: #2b6cb0;
  text-decoration: none;
}

.page_item a:hover {
  background-color: #e0e0e0;
}


.grandchild-sidebar-menu {
  margin-top: 10px;
  padding-left: 1.5rem;
}

.grandchild-sidebar-menu a {
  font-size: 0.9rem;
  padding: 6px 0;
}

.grandchild-sidebar-menu a:hover {
  background-color: #f5f5f5;
}

.current_page_item > a {
  font-weight: bold;
  color: #3182ce;
}

.bg-gray-200 {
  background-color: #edf2f7;
}

/* Flex Layout */
.flex {
  display: flex;
}


.p-6 {
  padding: 1.5rem;
}

.space-y-4 {
  margin-bottom: 1rem;
}
.relative {
  position: relative;
}

.underline-half::after {
  content: "";
  position: absolute;
  bottom: 0;
  left: 50%;
  width: 50%; /* This makes it cover half of the line */
  height: 2px;
  background-color: #2b6cb0; /* Blue underline color */
  transform: translateX(-50%); /* This centers the underline */
}

</style>
