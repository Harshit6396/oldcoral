<template>
  <fixedheader/>
  <div class="min-h-screen ">
    <section class="relative text-center pt-25 pb-25 bg-cover bg-center" style="background-image: url('/Contact-Us-1.jpg');">
      <!-- Overlay -->
      <div class="absolute inset-0 bg-[#34495e] opacity-75"></div>
      <!-- Content (ensure content is positioned above the overlay) -->
      <div class="relative">
        <h1 class="text-4xl font-bold text-white tracking-wide mb-2 relative inline-block">
          CONTACT US
          <!-- Blue Underline under the text -->
          <div class="absolute bottom-0 left-0 w-full h-0.5 bg-blue-500"></div>
        </h1>
        <div class="flex justify-center mt-2">

        </div>


        <h2 class="text-lg text-white">FEEL FREE TO GET IN TOUCH WITH US!</h2>
      </div>
    </section>
    <div class="container mx-auto px-5">
      <div class="grid grid-cols-1 md:grid-cols-2 gap-8 items-start mt-8">
        <div>
          <!-- Google Maps Embed -->
          <iframe
              class="rounded-lg w-full h-96 "
              src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d14009.355370421421!2d77.13952963430662!3d28.693410267914448!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x390d030ad9b6292d%3A0x7143c5538578056a!2sCoral%20Knowledge%20Services%20Pvt.%20Ltd!5e0!3m2!1sen!2sin!4v1634305952607!5m2!1sen!2sin"
              allowfullscreen=""
              loading="lazy"
              referrerpolicy="no-referrer-when-downgrade"></iframe>
        </div>
        <iframe
            src="https://tally.so/embed/3q9eEd"
            width="100%"
            height="500"
            frameborder="0"
            marginheight="0"
            marginwidth="0"
            class="rounded-lg shadow"
            allowtransparency="true"
            sandbox="allow-popups allow-popups-to-escape-sandbox allow-same-origin allow-scripts"
        ></iframe>
      </div>
    </div>
  </div>
  <Footer/>
</template>

<script setup>
import { reactive } from 'vue'

const form = reactive({
  name: '',
  email: '',
  mobile: '',
  country: '',
  comments: '',
  captcha: ''
})

function submitForm() {
  // Submit logic here
  alert('Form submitted!');
}
</script>
