<script setup lang="ts">
</script>
<template>
  <!-- Footer Component -->
  <div class="bg-[#262626] text-[#a9a9a9] py-12">
    <div class="max-w-7xl mx-auto px-4">
      <!-- Main Footer Content -->
      <div class="flex flex-wrap justify-between text-center">
        <!-- Contact Us Section -->
        <div class="w-full md:w-1/4 text-center mb-8 md:mb-0">
          <h3 class="text-white mb-4 tracking-wider">CONTACT US</h3>
          <div class="space-y-2 text-sm">
            <p class="font-medium">Coral Knowledge Services Pvt. Ltd.</p>
            <p>Unit 215 & 309,</p>
            <p>Aggarwal Prestige Mall,</p>
            <p>Road No. 44, Near M2K Pitampura,</p>
            <p>New Delhi-110034, India</p>
            <p>Mobile: +91-9212161176,</p>
            <p>+91-9212161170</p>
            <p>Phone: +91-11-47065658</p>
            <p>info@coralknowledgeservices.in</p>
          </div>
        </div>

        <!-- Social Media Section -->
        <div class="w-full md:w-1/4 flex justify-center mb-8 md:mb-0">
          <div class="bg-white border-2-white p-1 w-full h-70 overflow-hidden">
            <div class="flex items-center mb-3 gap-1" style="background: linear-gradient(to bottom, #000000b3, #0000);">
              <div class="w-14 h-14 flex items-center justify-center overflow-hidden border-2 border-white shadow-[0_1px_6px_#00000080] bg-white">
                <img src="/public/CORAL-NEW-LOGO.png" alt="Coral Knowledge Services" class="w-14 h-14 object-contain" />
              </div>
              <div>
                <p style="color: white;" class="text-sm">Coral Knowle...</p>

                <a
                    href="https://www.facebook.com/201054513303315?ref=embed_page"
                    target="_blank"
                    rel="noopener noreferrer"
                    class="inline-flex items-center gap-1 bg-white text-black text-xs px-2 py-1 rounded transition-colors"
                >
                  <div class="w-3 h-3 bg-blue-800 rounded-sm flex items-center justify-center">
                    <span class="text-white text-xs font-bold">f</span>
                  </div>
                  Follow Page
                </a>
              </div>
            </div>

            <!-- Social Media Content with Scrollable Area -->
            <div class="h-48 overflow-y-auto scrollbar-thin scrollbar-thumb-gray-300">
              <div class="space-y-3">
                <div class="border-b border-gray-100 pb-2">
                  <p class="text-xs text-gray-700 mb-1">We specialize in #language solutions for businesses...</p>
                  <div class="flex items-center gap-2 text-xs text-gray-500">
                    <span>👍 8</span>
                    <span>💬 3</span>
                    <span class="text-blue-600">Share</span>
                  </div>
                </div>

                <div class="border-b border-gray-100 pb-2">
                  <p class="text-xs text-gray-700 mb-1">
                    ✅ Marketing translation ✅ Website translation ✅ Legal documents...
                  </p>
                  <div class="flex items-center gap-2 text-xs text-gray-500">
                    <span>👍 2</span>
                    <span>💬 Comment</span>
                    <span class="text-blue-600">Share</span>
                  </div>
                </div>

                <div class="border-b border-gray-100 pb-2">
                  <p class="text-xs text-gray-700 mb-1">
                    Boost your brand value in Myanmar by delivering engaging experiences...
                  </p>
                  <div class="flex items-center gap-2 text-xs text-gray-500">
                    <span>👍 9</span>
                    <span>💬 2</span>
                    <span class="text-blue-600">Share</span>
                  </div>
                </div>

                <div class="pb-2">
                  <p class="text-xs text-gray-700 mb-1">
                    Contact us to see how you can take your product global! 📧 info@coralknowledgeservices.in
                  </p>
                  <div class="flex items-center gap-2 text-xs text-gray-500">
                    <span>👍 4</span>
                    <span>💬 1</span>
                    <span class="text-blue-600">Share</span>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>

        <!-- Tweets Section -->
        <div class="w-full md:w-1/4 text-sm text-gray-400 mb-8 md:mb-0">
          <p class="mb-4">
            <a href="https://x.com/rahulchhillar" target="_blank" class="text-gray-400 hover:text-white">
              Tweets by Rahul
            </a>
          </p>

          <!-- Tweets Section Content -->
          <div class="mt-4 space-y-2">
            <p class="text-gray-400">
              <a href="http://lnkd.in/AQSZm5" target="_blank" class="text-gray-400 hover:text-white">
                Top 10 Tips for Website Translation
              </a>
            </p>
            <p class="text-gray-400">
              <a href="http://lnkd.in/AQSZm5" target="_blank" class="text-gray-400 hover:text-white">
                Tips for Translation and Regulatory Compliance in the Pharmaceutical and Medical Device Industries
              </a>
            </p>
            <p class="text-gray-400">
              <a href="http://lnkd.in/AQSZm5" target="_blank" class="text-gray-400 hover:text-white">
                Coral Knowledge Unveils Localisation Services https://lnkd.in/fbbhHpE
              </a>
            </p>
            <p class="text-gray-400">
              <a href="http://lnkd.in/JctHr7" target="_blank" class="text-gray-400 hover:text-white">
                The global market for outsourced language services and technology will reach US$33.523 billion in 2012 and is growing…
              </a>
            </p>
          </div>
        </div>

        <!-- Newsletter Section -->
        <div class="w-full md:w-1/4">
          <h3 class="text-white mb-4 tracking-wider">
            SIGN UP FOR OUR
            <br />
            NEWSLETTER!
          </h3>
          <div class="space-y-4">
            <div>
              <label for="email" class="block text-sm mb-2">
                Email Address:
              </label>
              <input
                  id="email"
                  v-model="email"
                  type="email"
                  class="w-full bg-white border border-gray-300 text-gray-800 px-3 py-2 rounded focus:outline-none focus:ring-2 focus:ring-blue-500"
                  placeholder="Enter your email"
              />
            </div>
            <button
                @click="signUp"
                class="bg-blue-600 hover:bg-blue-700 text-white px-6 py-2 rounded-full transition-colors font-medium"
            >
              SIGN UP
            </button>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Bottom Footer -->
  <div class="border-t border-gray-700 mx-auto p-6 bg-[#1b1b1b]">
    <div class="flex flex-col md:flex-row mx-auto justify-center items-center gap-4 text-center">
      <div class="text-sm text-gray-400">
        <p>Copyright © 2020 Coral Knowledge Services Pvt. Ltd.</p>
        <p>All Rights Reserved</p>
      </div>
      <div class="flex flex-wrap gap-4 text-sm">
        <a href="#" class="text-gray-400 hover:text-white">
          Privacy Policy
        </a>
        <span class="text-gray-600">|</span>
        <a href="#" class="text-gray-400 hover:text-white">
          Terms & Conditions
        </a>
        <span class="text-gray-600">|</span>
        <a href="#" class="text-gray-400 hover:text-white">
          Sitemap
        </a>
      </div>
      <div>
        <a href="#" class="text-gray-400 hover:text-white text-sm font-medium">
          GO TO TOP ▲
        </a>
      </div>
    </div>
  </div>
  <!-- Footer Component -->
</template>

<style scoped>
/* Custom scrollbar styles */
.scrollbar-thin::-webkit-scrollbar {
  width: 4px;
}

.scrollbar-thumb-gray-300::-webkit-scrollbar-thumb {
  background-color: #d1d5db;
  border-radius: 2px;
}

.scrollbar-thin::-webkit-scrollbar-track {
  background-color: transparent;
}
.w-full.md\:w-1\/4.text-sm.text-gray-400.mb-8.md\:mb-0 {
  padding-left: 20px;
  padding-right: 20px;
}
</style>
