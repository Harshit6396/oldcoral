<template>
  <Fixedheader/>
  <div>
    <!-- Header with background image -->
    <div
        class="h-80 flex items-center justify-center bg-cover bg-center relative"
        :style="'background-image: url(/pro.jpg)'"
    >
      <!-- Overlay -->
      <div class="absolute inset-0 bg-[#34495e] opacity-75"></div>

      <!-- Text with blue line -->
      <h1 class="text-5xl text-white font-bold tracking-wide drop-shadow-lg relative z-10">
        PROCESS
        <!-- Blue Underline under the text -->
        <span class="block w-full h-0.5 bg-blue-500 mt-2 mx-auto"></span>
      </h1>



    </div>


    <!-- Main content section -->
    <div class="container mx-auto px-4 py-12 flex flex-col items-center">
      <h2 class="font-semibold mb-4">The Translation Process – Achieve the Best Results
      </h2>
      <!-- Process overview description (optional, add/change as per your content) -->
      <p class="max-w-5xl text-left text-gray-600 mb-12">
        Because Coral Knowledge Services works on an ongoing basis with multiple clients, producing multiple documents in multiple languages requiring multiple translators, our organizational skills are enviable. This strict attention to detail and organizational effectiveness allows us to successfully compete with all other translation companies. We actively create, view and manage project management tools so that at any point in the process you can trace exactly where we are on every one of your projects. This incredible project management style helps us produce efficiencies that virtually eliminate mistakes and enables us to meet or beat all of our clients’ timelines, deadlines, and budgets.


      </p>

      <!-- Central process image -->
      <img
          src="/cks-process.jpg"
          alt="Coral Knowledge Services Translation Process"
          class="mx-auto my-8 max-w-full md:max-w-3xl object-contain shadow-lg"
      />

      <!-- Below-image content (you can add further details, steps, etc.) -->
      <div class="max-w-5xl text-gray-700 text-sm">
        <h2 class="font-semibold mb-4">All Your Translations Are Guaranteed!</h2>
        <p class="mb-6">
          We stand by all translations completed by our translators. We will correct any verifiable translation errors committed by our translators free of charge for a period of sixty (60) days. Stylistic changes (including terminology preferences not communicated to Coral Knowledge Services Pvt. Ltd. prior to the start of the translation) are not covered by the guarantee and will be subject to additional charges.
        </p>

        <h3 class="font-semibold mb-4">Processing Customer Enquiry</h3>
        <ul class="list-disc list-inside space-y-2 mb-6">
          <li>Our potential client sends inquiries through email or web form or through online chat.</li>
          <li>The inquiry is classified according to the language pair, duration, translator availability, specialization, and a few other parameters.</li>
          <li>Once the inquiry is qualified, it is pushed to the project manager for immediate action.</li>
          <li>The project manager generates an automatic quote from our CRM and sends it to the customer for approval with the justification to cost, timeline, validity, etc.</li>
          <li>On receiving the quotation our client either calls to confirm the status or sends in the mail to confirm.</li>
          <li>Both are recorded in our CRM for further action. This way we also keep track of the client and inquiry history for future use.</li>
        </ul>

        <h3 class="font-semibold mb-4">Processing Customer Orders</h3>
        <p class="mb-6">
          The customer service efficiency of any company is directly linked to its customer order management efficiency. We handle hundreds of translation requests on a daily basis from as many customers from more than 35 countries. Our custom-built order management solution handles our sales orders and accounts for optimized fulfillment of all incoming orders.
        </p>

        <h3 class="font-semibold mb-4">Listed below is the process we follow in handling each and every inquiry on a day-to-day basis.</h3>
        <ul class="list-disc list-inside space-y-2 mb-6">
          <li>Our clients forward the approval based on our quotation.</li>
          <li>Some of our clients request samples to see if the translation suits them or to test our skills. We promptly respond to such requests and send them. We also send in translator profiles for clients to be sure of our capability.</li>
          <li>Once the client approves the quotation or sample, Coral Knowledge Services will get the document translated.</li>
          <li>Coral will check for the file format, quotation, etc., generate a progress sheet using our project management software and share that with our clients and then assign the work to the translators.</li>
          <li>We also transmit the files for translation through FTP, a secure process to ensure the files reach the translators without any vulnerability.</li>
          <li>We monitor the progress of translation at each and every step to ensure there is work happening from the time it is assigned.</li>
          <li>As we are aware of the high reliance on individuals in different locations, we take proper contingency measures and track the progress every hour and day to avoid delays or issues during the deliveries.</li>
          <li>Once the files are received from the translators, it is sent to the proofreaders who are identified to do while receiving the order. Once the proofreading is done, it is sent to the in-house team to do a document validation to check if all the pages or graphics, or diagrams are pagination is in order. Required fonts, etc are present and it is ready for delivery.</li>
          <li>We transmit the files along with the invoice for processing payment from the client's side.</li>
          <li>If the client has any issues with the translation, we enable a conference call with the translator and the project team for them to discuss and sort out.</li>
          <li>We sign NDAs and SLAs as per the client’s requirement.</li>
        </ul>

        <strong>Hope you are satisfied with the information to arrive at a decision.</strong>
        <p class="mb-2">
          To evaluate and decide on the right translation company for you, use our live support to talk to our Project Managers or you can also mail us at
          <span class="text-blue-600">info@coralknowledgeservices.in</span> or Call us at <span class="text-blue-600">+91(011) 45696558</span> for information.
        </p>
      </div>
    </div>
  </div>
  <Footer/>
</template>

<script setup>
// No JS logic required for this static layout
</script>
