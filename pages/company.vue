<template>
  <Fixedheader/>
  <div>
    <!-- Hero Section -->
    <div
        class="relative h-[360px] w-full flex items-center justify-center text-white"
        :style="{ backgroundImage: 'url(/homepage.jpg)', backgroundSize: 'cover', backgroundPosition: 'center' }"
    >
      <div class="absolute inset-0" style="background-color: #34495e; opacity: 0.75;"></div>
      <div class="relative z-10 text-center w-full">
        <h1 class="relative inline-block text-5xl font-bold mb-4 tracking-wide uppercase">
          ABOUT US
          <!-- Full Blue Underline under the text -->
          <div class="w-full h-[3px] bg-blue-500 mt-2 mx-auto"></div>
        </h1>

        <h2 class=" text-l text-white">MEET OUR TEAM</h2>
      </div>

    </div>


    <!-- Achievements Section -->
    <section class="py-12 bg-gray-50">
      <h2 class="text-center text-lg font-semibold mb-8">OUR AMAZING ACHIEVEMENTS</h2>
      <div class="flex justify-center gap-14 text-center max-w-4xl mx-auto">
        <div class="flex flex-col items-center">
          <div class="mb-2 text-3xl">
            <img src="https://i.ibb.co/RGWS3Db8/globe.png" alt="Globe" class="w-12 h-12" />
          </div>
          <div class="relative inline-block text-6xl font-bold counter" data-target="2009">
            0
          </div>
          <div class="mt-1 text-gray-500 text-sm">Company was established</div>
        </div>

        <div class="flex flex-col items-center">
          <div class="mb-2 text-3xl">
            <img src="https://i.ibb.co/VYHnCwR6/pencil.png" alt="heart" class="w-12 h-12" />
          </div>
          <div class="relative inline-block text-6xl font-bold counter" data-target="79">
            0
          </div>
          <div class="mt-1 text-gray-500 text-sm">Millions words Translated</div>
        </div>

        <!-- Apply k-counter class for 72k formatting -->
        <div class="flex flex-col items-center">
          <div class="mb-2 text-3xl">
            <img src="https://i.ibb.co/mrHHX0D4/heart.png" alt="heart" class="w-12 h-12" />
          </div>
          <div class="relative inline-block text-6xl font-bold counter k-counter" data-target="72000">
            0
          </div>
          <div class="mt-1 text-gray-500 text-sm">Projects We have Worked on</div>
        </div>

        <!-- Apply plus-counter class for 4000+ formatting -->
        <div class="flex flex-col items-center">
          <div class="mb-2 text-3xl">
            <img src="https://i.ibb.co/N6VX4Rt6/coffee.png" alt="cup" class="w-12 h-12" />
          </div>
          <div class="relative inline-block text-6xl font-bold counter plus-counter" data-target="4000">
            0
          </div>

          <div class="mt-1 text-gray-500 text-sm">Native Translators</div>
        </div>
      </div>
    </section>

    <!-- Team Section -->
    <section class="py-16 bg-white">
      <h2 class="text-center text-lg font-semibold mb-12">MEET OUR TEAM</h2>
      <div class="flex justify-center gap-8 flex-wrap">
        <!-- Team Member 1 -->
        <div class="bg-gray-50 shadow rounded-lg p-6 flex flex-col items-center w-64">
          <img src="/rahulchillar.jpg" alt="Rahul Chillar" class="w-35 h-35 rounded mb-4" />
          <h3 class="font-bold text-md">RAHUL CHILLAR</h3>
          <div class="text-sm text-gray-700 mb-2">Director</div>
          <p class="text-sm text-gray-600 text-center">
            Rahul is responsible for exploring the business opportunities for Coral. He studied at Delhi College of Engineering and holds an MBE degree (Delhi University) in Marketing and Finance. Rahul is also responsible for all financial matters.
          </p>
        </div>

        <!-- Team Member 2 -->
        <div class="bg-gray-50 shadow rounded-lg p-6 flex flex-col items-center w-64">
          <img src="/anjalitaneja.jpg" alt="Anjali Taneja" class="w-35 h-35 rounded mb-4" />
          <h3 class="font-bold text-md">ANJALI TANEJA</h3>
          <div class="text-sm text-gray-700 mb-2">Group Manager</div>
          <p class="text-sm text-gray-600 text-center">
            Anjali heads the highly talented and experienced project management team. She is responsible for day-to-day translation operations and manages the translation, project management, resource management and compliance teams.
          </p>
        </div>

        <!-- Team Member 3 -->
        <div class="bg-gray-50 shadow rounded-lg p-6 flex flex-col items-center w-64">
          <img src="/kaushik.jpg" alt="Kaushik N" class="w-35 h-35 rounded mb-4" />
          <h3 class="font-bold text-md">KOUSHIK N</h3>
          <div class="text-sm text-gray-700 mb-2">Project Manager</div>
          <p class="text-sm text-gray-600 text-center">
            Koushika is responsible for client communication and project deliveries. She also maintains relations with our current clients to ensure they continue to receive the best possible service. She is in charge of the daily Workflow and makes sure the QA Procedures are met.
          </p>
        </div>

        <!-- Team Member 4 -->
        <div class="bg-gray-50 shadow rounded-lg p-6 flex flex-col items-center w-64">
          <img src="/richa.jpg" alt="Richa Singh" class="w-35 h-35 rounded mb-4" />
          <h3 class="font-bold text-md">RICHA SINGH</h3>
          <div class="text-sm text-gray-700 mb-2">Asst. Project Manager</div>
          <p class="text-sm text-gray-600 text-center">
            Richa specializes in editing texts produced by other translators to enhance readability and impact. She has been working at coral since 2018. She is responsible for maintaining our ISO standard procedures and documentation.
          </p>
        </div>
      </div>
    </section>
  </div>

<worked/>
  <Footer/>
</template>

<script>
export default {
  mounted() {
    const counters = document.querySelectorAll('.counter');

    counters.forEach(counter => {
      const target = +counter.getAttribute('data-target');
      let current = +counter.innerText;
      const increment = target / 100; // Adjust the speed of counting here

      const isKCounter = counter.classList.contains('k-counter'); // Check if it's the 72k counter
      const isPlusCounter = counter.classList.contains('plus-counter'); // Check if it's the 4000+ counter

      const updateCounter = () => {
        if (current < target) {
          current = Math.ceil(current + increment);
          counter.innerText = isKCounter ? formatNumber(current) : isPlusCounter ? formatPlus(current) : current;
          requestAnimationFrame(updateCounter);
        } else {
          counter.innerText = isKCounter ? formatNumber(target) : isPlusCounter ? formatPlus(target) : target;
        }
      };

      // Initial call
      updateCounter();
    });

    // Function to format numbers as k (lowercase)
    function formatNumber(num) {
      if (num >= 1000) {
        return (num / 1000).toFixed(0) + 'k'; // Format as 72k
      }
      return num;
    }

    // Function to add + symbol for the 4000+ counter
    function formatPlus(num) {
      return num + '+';
    }
  }
}
</script>




<style>
.counter {
  position: relative;
  display: inline-block;
}

.counter::after {
  content: '';
  display: block;
  width: 100%;  /* Adjust the width as needed */
  height: 3px;  /* Height of the blue line */
  background-color: #3498db;  /* Blue color */
  margin: 10px auto 0;  /* Centers the underline and adds some spacing */
}

</style>
