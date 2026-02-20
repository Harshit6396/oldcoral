<template>
  <fixedheader/>
  <div class="min-h-screen">
    <!-- Header Section with Background and Overlay -->
    <section
        class="text-center pt-25 pb-25 bg-cover bg-center relative"
        style="background-image: url('/Contact-Us-1.jpg');"
    >
      <div class="absolute inset-0 bg-[#34495e] opacity-75"></div>
      <div class="relative">
        <h1 class="text-4xl font-bold text-white tracking-wide mb-2 relative inline-block">
          CAREERS
          <!-- Blue Underline under the text -->
          <div class="absolute bottom-0 left-0 w-full h-0.5 bg-blue-500"></div>
        </h1>

        <p class="text-lg text-gray-200">WANT TO WORK WITH US? JOIN US NOW!</p>
      </div>
    </section>

    <!-- Main Content Grid -->
    <div class="container mx-auto px-5 py-10 grid grid-cols-1 md:grid-cols-2 gap-12 max-w-7xl">

      <!-- Left Text Section -->
      <div class="text-gray-800 text-sm leading-relaxed">
        <h2 class="font-bold uppercase mb-4 text-md">
          DO YOU HAVE A PASSION FOR LANGUAGES, CULTURES, AND TECHNOLOGY?
        </h2>

        <p class="mb-4">
          We are always seeking outstanding and diverse candidates with a wide range of backgrounds to help our clients work more effectively in the global marketplace. If you are passionate about languages and technology, we invite you to become part of our dynamic team. With our rapid growth, you’ll find no shortage of opportunities for advancement. Coral Knowledge Services is a rewarding place to work, and the deliverables we produce every day can impact the success or failure of our clients’ global initiatives.
        </p>

        <p class="mb-4">
          If you think you’ve got what it takes to join the most enthusiastic, quality-oriented, and client-focused team in the language industry, drop us a line.
        </p>

        <p class="mb-4">
          We invite you to contact us today for any of the career opportunities listed below:
        </p>

        <ul class="list-disc ml-6 mb-4">
          <li>Translator for Hindi, Punjabi, and Telugu Translator (full-time positions)</li>
          <li>Editor for Hindi, Urdu, Tamil, and Bengali (India)</li>
          <li>Localization Project Manager (over 4 years of localization experience)</li>
        </ul>

        <p class="mb-4">
          The New Delhi Office is looking for a bright intern to support our Team of Language Professionals, Editors, and Proofreaders. Apply today and write an email with your CV and Cover Letter to <a href="mailto:hr@coralknowledgeservices.in" class="text-blue-600 underline">hr@coralknowledgeservices.in</a>.
        </p>

        <p class="font-semibold uppercase">GO GLOBAL WITH CORAL!!</p>
      </div>

      <!-- Right Tally Form Embed Section -->
      <div>
        <iframe
            src="https://tally.so/r/3xABRE"
            width="100%"
            height="640"
            frameborder="0"
            marginheight="0"
            marginwidth="0"
            class="rounded-lg shadow-lg"
            allowtransparency="true"
            sandbox="allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts"
        ></iframe>
      </div>
    </div>
  </div>
  <Footer />
</template>
<style>
.underline-careers {
  position: relative;
  display: inline-block;
}

.underline-careers::after {
  content: '';
  display: block;
  width: 50%;  /* Adjust the width as needed */
  height: 3px;  /* Height of the blue line */
  background-color: #3498db;  /* Blue color */
  margin: 10px auto 0;  /* Centers the underline and adds some spacing */
}
</style>
