<template>
  <fixedheader/>
  <div class="min-h-screen bg-gray-50">
    <!-- Header Section with Background Image -->
    <section
        class="relative h-64 bg-cover bg-center bg-no-repeat flex items-center justify-center"
        :style="{ backgroundImage: 'url(/pulication.jpg)' }"
    >
      <!-- Overlay -->
      <div class="absolute inset-0 bg-black opacity-50 z-0"></div> <!-- Dark overlay with 50% opacity -->

      <!-- Content -->
      <div class="relative z-10 text-center">
        <h1 class="text-4xl font-bold text-white tracking-wider">
    <span class="relative inline-block">
      TECHNICAL PUBLICATIONS
      <!-- Underline under the text -->
      <div class="absolute bottom-0 left-0 w-full h-0.5 bg-blue-400"></div>
    </span>
        </h1>
      </div>

    </section>


    <!-- Main Content -->
    <div class="max-w-7xl mx-auto px-4 py-12">
      <div class="grid grid-cols-1 lg:grid-cols-4 gap-8">
        <!-- Sidebar Navigation -->


        <!-- Main Content Area -->
        <div class="lg:col-span-4">
          <!-- Introduction Text -->
          <div class="text-center mb-12">
            <p class="text-gray-600 max-w-4xl mx-auto leading-relaxed">
              Our technical publications provide comprehensive documentation, research findings, and industry insights.
              These resources are designed to support professionals, researchers, and organizations in their technical endeavors.
            </p>
          </div>

          <!-- Publication Previews -->
          <div class="grid md:grid-cols-3 gap-8 mb-16">
            <div class="bg-white border border-gray-200 rounded-lg p-6 shadow-sm">
              <div class="bg-blue-600 text-white px-3 py-1 text-sm rounded mb-4 inline-block">
                Technical Report
              </div>
              <h3 class="font-semibold text-gray-800 mb-3">Advanced Systems Analysis</h3>
              <ul class="text-sm text-gray-600 space-y-2">
                <li>• System Architecture Overview</li>
                <li>• Performance Metrics</li>
                <li>• Implementation Guidelines</li>
                <li>• Best Practices</li>
              </ul>
            </div>

            <div class="bg-white border border-gray-200 rounded-lg p-6 shadow-sm">
              <div class="bg-blue-600 text-white px-3 py-1 text-sm rounded mb-4 inline-block">
                Research Paper
              </div>
              <h3 class="font-semibold text-gray-800 mb-3">Innovation Methodologies</h3>
              <ul class="text-sm text-gray-600 space-y-2">
                <li>• Research Framework</li>
                <li>• Data Analysis Methods</li>
                <li>• Case Studies</li>
                <li>• Future Directions</li>
              </ul>
            </div>

            <div class="bg-white border border-gray-200 rounded-lg p-6 shadow-sm">
              <div class="bg-blue-600 text-white px-3 py-1 text-sm rounded mb-4 inline-block">
                White Paper
              </div>
              <h3 class="font-semibold text-gray-800 mb-3">Industry Standards</h3>
              <ul class="text-sm text-gray-600 space-y-2">
                <li>• Compliance Requirements</li>
                <li>• Quality Assurance</li>
                <li>• Regulatory Guidelines</li>
                <li>• Implementation Roadmap</li>
              </ul>
            </div>
          </div>

          <!-- Domains Section -->
          <section class="mb-16">
            <h2 class="text-2xl font-bold text-gray-800 mb-8 text-center">DOMAINS</h2>
            <div class="grid md:grid-cols-3 gap-8">
              <div class="text-center">
                <div class="w-16 h-16 bg-blue-100 rounded-full flex items-center justify-center mx-auto mb-4">
                  <span class="text-blue-600 text-2xl">🔧</span>
                </div>
                <h3 class="font-semibold text-gray-800 mb-2">Engineering</h3>
                <p class="text-sm text-gray-600">Advanced engineering solutions and methodologies</p>
              </div>
              <div class="text-center">
                <div class="w-16 h-16 bg-blue-100 rounded-full flex items-center justify-center mx-auto mb-4">
                  <span class="text-blue-600 text-2xl">💻</span>
                </div>
                <h3 class="font-semibold text-gray-800 mb-2">Technology</h3>
                <p class="text-sm text-gray-600">Cutting-edge technology research and development</p>
              </div>
              <div class="text-center">
                <div class="w-16 h-16 bg-blue-100 rounded-full flex items-center justify-center mx-auto mb-4">
                  <span class="text-blue-600 text-2xl">📊</span>
                </div>
                <h3 class="font-semibold text-gray-800 mb-2">Analytics</h3>
                <p class="text-sm text-gray-600">Data analytics and business intelligence</p>
              </div>
            </div>
          </section>

          <!-- Service Offerings Section -->
          <!-- Service Offerings Section -->
          <section class="mb-16">
            <h2 class="text-2xl font-bold text-gray-800 mb-8">SERVICE OFFERINGS</h2>
            <div class=" rounded-lg  ">
              <p class="text-gray-600 mb-6 leading-relaxed">
                In a modern dynamic environment of complex technologies and equipment, timely access to accurate, mission-critical technical information is indispensable to ensure streamlined operations, service, regulatory compliance, and most importantly, safety. The team at Coral possesses in-depth experience in the Automotive, Aerospace, Heavy Machinery & Oil, and Gas domain, and offers comprehensive part-to-part Technical Documentation solutions for the Aerospace, Automotive, Heavy Engineering Machinery, Discrete, Process, and other engineering industries.
              </p>

              <p class="text-gray-600 mb-6 leading-relaxed">
                This Competency development capability of Coral helps to provide technical, reliable, and sustainable high-tech engineering services using CAD, CAE, PLM. Rapid prototyping, technical publications, and embedded solutions in the field of aerospace, automotive, defense, product design, medical engineering, and general engineering industries. Coral utilizes internal resources skilled by the competency development program which is cost-effective & high-quality deliverable.
              </p>

              <p class="text-gray-600 mb-6 leading-relaxed">
                Coral culminates multi-domain knowledge and experience in Technical Writing, Illustration, Animation, and Translation of Technical Documents. We offer cost-effective, quality documentation deliver on time. Our Technical Publication service also supports industry-wide documentation standards such as ATA100, ATA iSpec 2200, ASD Simplified Technical (STE), Chicago Manual of Style, Microsoft Manual of Style Guide, AICC & SCORM standards. A client using our service can quickly adapt legacy publications to the latest standards required by the industry.
              </p>

              <h4 class="font-semibold text-gray-800 mb-3">Coral offers the creation and modification of the following manuals:</h4>
              <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                <ul class="text-sm text-gray-600 space-y-2">
                  <li>• Illustrated Parts Manuals</li>
                  <li>• Maintenance Manuals</li>
                  <li>• Aircraft Maintenance Manual (AMM)</li>
                  <li>• Component Maintenance Manual (CMM)</li>
                  <li>• Structural Repair Manual (SRM)</li>
                  <li>• Service Bulletins (SBs)</li>
                  <li>• Job Cards</li>

                </ul>
                <ul class="text-sm text-gray-600 space-y-2">
                  <li>• Temporary Revisions (TRs)</li>
                  <li>• Pilots Handbook</li>
                  <li>• Flight Manual</li>
                  <li>• Operators Manual</li>
                  <li>• Ground Support Equipment Manual</li>
                  <li>• Legacy conversion of documents into SGML- and/or XML-based environments</li>
                </ul>
                <ul class="text-sm text-gray-600 space-y-2">
                  <li>• Interactive Electronic Technical Manuals (IETM)</li>
                  <li>• Computer Based Training Manuals (CBT)</li>
                  <li>• Web-Based Training Materials (WBTSM)</li>
                  <li>• Tool & Equipment Manual</li>
                  <li>• E-Catalogue</li>
                  <li>• Service Manual</li>
                  <li>• MP</li>
                </ul>
              </div>

            </div>
          </section>


          <!-- Key Benefits Section -->
          <section class="mb-16">
            <h2 class="text-2xl font-bold text-gray-800 mb-8">KEY BENEFITS</h2>
            <ul class="text-sm text-gray-600 space-y-2 mb-8">
              <li>• Domain Expertise: Skills in Automotive, Aerospace, Heavy Machinery, Process, and Discrete domains with expertise in a wide range of tools</li>
              <li>• Quality Standards: Meticulous knowledge of Aerospace standards, such as Air Transport Association’s ATA100, ATA iSpec2200, MTOSS, Association of European Aircraft and Component Manufacturers (AECMA) S1000D and ASD-STE100</li>
              <li>• Process Maturity: Strict consistent processes, style sheets, controls for on-time delivery, and accurate technical documentation</li>
              <li>• Reduced Costs: Established delivery model optimizes costs for the lifecycle of Auto Financial Services</li>
              <li>• Flexible Delivery Model: A global delivery model can match customers' footprint across the globe</li>
              <li>• Elimination of Redundancy: Minimize rewriting and recreation of content through streamlined review, validation, and approval processes</li>
            </ul>
            <div class="grid md:grid-cols-2 gap-8">

              <div class="bg-white rounded-lg p-6 shadow-sm border border-gray-200">
                <h3 class="font-semibold text-gray-800 mb-4">OUR COMPETENCIES</h3>
                <ul class="text-sm text-gray-600 space-y-2">
                  <li>• Expert technical writing team</li>
                  <li>• Industry-specific knowledge</li>
                  <li>• Quality assurance processes</li>
                  <li>• Regulatory compliance expertise</li>
                  <li>• Multi-format publishing capabilities</li>
                  <li>• Collaborative development approach</li>
                </ul>
              </div>

              <div class="bg-white rounded-lg p-6 shadow-sm border border-gray-200">
                <h3 class="font-semibold text-gray-800 mb-4">OTHER SPECIALIZED SERVICES</h3>
                <ul class="text-sm text-gray-600 space-y-2">
                  <li>• Custom documentation solutions</li>
                  <li>• Multilingual publication support</li>
                  <li>• Digital transformation consulting</li>
                  <li>• Content strategy development</li>
                  <li>• Training and workshops</li>
                  <li>• Ongoing maintenance and updates</li>
                </ul>
              </div>
            </div>
            <p class="text-sm text-gray-600 mb-8 mt-8">We enjoy exploring new opportunities and would be interested in discussing your specific requirements. Contact us today to see how we can serve your needs.<br>
              <a href="mailto:info@coralknowledgeservices.in">info@coralknowledgeservices.in</a>
            </p>
          </section>
        </div>
      </div>
    </div>
  </div>
  <Footer />
</template>

<script setup>
import { useHead } from '#app';

// Set page meta using Nuxt 3's auto-imported useHead composable
useHead({
  title: 'Technical Publications',
  meta: [
    { name: 'description', content: 'Comprehensive technical publications and documentation services' }
  ]
})
</script>

<style scoped>
/* Additional custom styles if needed */
</style>