<template>
  <header class="bg-white shadow-sm">
    <!-- Top bar with contact info and social links -->
    <div class="bg-gray-50 border-b border-gray-200">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="flex justify-between items-center py-2 text-sm text-gray-600">
          <!-- Contact Info -->
          <div class="flex items-center space-x-6">
            <div class="flex items-center">
              <Icon name="ph:phone" class="w-4 h-4 mr-2" />
              <span>+91 9818681169</span>
            </div>
            <div class="flex items-center">
              <Icon name="ph:envelope" class="w-4 h-4 mr-2" />
              <span>info@coralknowledgeservices.in</span>
            </div>
          </div>

          <!-- Search and Social -->
          <div class="flex items-center space-x-4">
            <!-- Search Bar -->
            <div class="relative">
              <input
                  v-model="searchQuery"
                  type="text"
                  placeholder="Search"
                  class="pl-8 pr-4 py-1 text-sm border border-gray-300 rounded-md focus:outline-none focus:ring-2 focus:ring-blue-500 focus:border-transparent"
                  @keyup.enter="handleSearch"
              />
              <Icon name="ph:magnifying-glass" class="absolute left-2 top-1/2 transform -translate-y-1/2 w-4 h-4 text-gray-400" />
            </div>

            <!-- Social Media Icons -->
            <div class="flex items-center space-x-2">
              <a href="https://twitter.com/rahulchhillar" class="text-gray-400 hover:text-blue-500 transition-colors">
                <Icon name="ph:twitter-logo" class="w-4 h-4" />
              </a>
              <a href="https://www.facebook.com/coralknowledgeservices" class="text-gray-400 hover:text-blue-600 transition-colors">
                <Icon name="ph:facebook-logo" class="w-4 h-4" />
              </a>
              <a href="https://www.linkedin.com/in/rahulchhillar" class="text-gray-400 hover:text-blue-700 transition-colors">
                <Icon name="ph:linkedin-logo" class="w-4 h-4" />
              </a>
              <a href="https://plus.google.com/115861507188488190716/posts" class="text-gray-400 hover:text-red-500 transition-colors">
                <Icon name="ph:google-logo" class="w-4 h-4" />
              </a>
            </div>
          </div>
        </div>
      </div>
    </div>

    <!-- Main header with logo and navigation -->
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <div class="flex justify-between items-center">
        <!-- Logo -->
        <NuxtLink to="/" class="flex-shrink-0">
          <!-- Replaced text-based logo with actual logo image -->
          <img
              src="/CORAL-NEW-LOGO.png"
              alt="Coral Knowledge Services"
              class="h-16 w-auto"
          />
        </NuxtLink>

        <!-- Desktop Navigation -->
        <nav class="hidden lg:flex items-center space-x-8">
          <!-- Enhanced navigation with both hover and click functionality -->
          <div
              v-for="item in navigationItems"
              :key="item.name"
              class="relative group"
              @mouseenter="showDropdown(item.name)"
              @mouseleave="hideDropdown"
          >
            <!-- Modified to handle parent items with both href and children -->
            <div v-if="item.children" class="flex items-center">
              <NuxtLink
                  :to="item.href"
                  class="text-gray-700 hover:text-blue-600 font-medium text-sm uppercase tracking-wide transition-colors"
                  :class="{ 'text-blue-600': $route.path === item.href }"
              >
                {{ item.name }}
              </NuxtLink>
              <button
                  @click="toggleDropdown(item.name)"
                  class="text-gray-700 hover:text-blue-600 font-medium text-sm uppercase tracking-wide transition-colors focus:outline-none ml-1"
              >
                <Icon name="ph:caret-down" class="w-4 h-4" />
              </button>
            </div>

            <!-- For items without children -->
            <NuxtLink
                v-else
                :to="item.href"
                class="text-gray-700 hover:text-blue-600 font-medium text-sm uppercase tracking-wide transition-colors"
                :class="{ 'text-blue-600': $route.path === item.href }"
            >
              {{ item.name }}
            </NuxtLink>

            <!-- Dropdown Menu -->
            <div
                v-if="item.children && activeDropdown === item.name"
                class="absolute top-full left-0 mt-1 w-64 bg-white border border-gray-200 shadow-lg rounded-md z-50"
                @mouseenter="keepDropdownOpen"
                @mouseleave="hideDropdown"
            >
              <div class="py-2">
                <NuxtLink
                    v-for="child in item.children"
                    :key="child.name"
                    :to="child.href"
                    class="block px-4 py-2 text-sm text-gray-700 hover:text-blue-600 hover:bg-gray-50 transition-colors uppercase tracking-wide"
                    @click="handleChildNavigation(child.href)"
                >
                  {{ child.name }}
                </NuxtLink>
              </div>
            </div>
          </div>
        </nav>

        <!-- Mobile menu button -->
        <button
            @click="mobileMenuOpen = !mobileMenuOpen"
            class="lg:hidden inline-flex items-center justify-center p-2 rounded-md text-gray-700 hover:text-blue-600 hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-inset focus:ring-blue-500"
        >
          <Icon :name="mobileMenuOpen ? 'ph:x' : 'ph:list'" class="w-6 h-6" />
        </button>
      </div>
    </div>

    <!-- Mobile Navigation Menu -->
    <div v-show="mobileMenuOpen" class="lg:hidden border-t border-gray-200 bg-white">
      <div class="px-4 py-2 space-y-1">
        <!-- Modified mobile navigation to handle parent links properly -->
        <div v-for="item in navigationItems" :key="item.name" class="space-y-1">
          <div class="flex items-center justify-between">
            <NuxtLink
                :to="item.href"
                class="flex-1 px-3 py-2 text-gray-700 hover:text-blue-600 hover:bg-gray-50 font-medium text-sm uppercase tracking-wide transition-colors rounded-md"
                :class="{ 'text-blue-600 bg-blue-50': $route.path === item.href }"
                @click="handleMobileParentNavigation(item)"
            >
              {{ item.name }}
            </NuxtLink>
            <button
                v-if="item.children"
                @click="toggleMobileSubmenu(item.name)"
                class="p-2 text-gray-400 hover:text-gray-600"
            >
              <Icon :name="expandedMobileMenus.includes(item.name) ? 'ph:caret-up' : 'ph:caret-down'" class="w-4 h-4" />
            </button>
          </div>

          <!-- Mobile Submenu -->
          <div v-if="item.children && expandedMobileMenus.includes(item.name)" class="pl-4 space-y-1">
            <NuxtLink
                v-for="child in item.children"
                :key="child.name"
                :to="child.href"
                class="block px-3 py-2 text-sm text-gray-600 hover:text-blue-400 transition-colors rounded-md uppercase tracking-wide"
                @click="handleMobileChildNavigation(child.href)"
            >
              {{ child.name }}
            </NuxtLink>
          </div>
        </div>
      </div>
    </div>
  </header>
</template>

<script setup>
import { ref, watch, onMounted, onUnmounted } from 'vue'
import { useRoute, navigateTo } from '#app'

const searchQuery = ref('')
const mobileMenuOpen = ref(false)
const activeDropdown = ref('')
const expandedMobileMenus = ref([])
const dropdownTimeout = ref(null)

const navigationItems = [
  {
    name: 'COMPANY',
    href: '/company',
    children: [
      { name: 'Why Us', href: '/why-us' }
    ]
  },
  {
    name: 'OFFERING',
    href: '/offering',
    children: [
      { name: 'Technical Publications', href: '/technical-publications' },
      { name: 'Translation Services', href: '/translation-services' },
      { name: 'Transcription Services', href: '/transcription-services' },
      { name: 'Interpreting Services', href: '/interpretation-services' },
      { name: 'Audio Visual Services', href: '/audio-visual-services' },
      { name: 'Data Capture Services', href: '/data-capture-services' }
    ]
  },
  {
    name: 'PROCESS',
    href: '/process',
    children: [
      { name: 'Languages we Translate', href: '/languages-we-translate' },
      { name: 'Multiple Languages', href: '/multiple-language-translation' },
      { name: "FAQ's", href: '/faqs-frequently-asked-questions' }
    ]
  },
  {
    name: 'INDUSTRIES',
    href: '/industries',
    children: [
      { name: 'Automotive Industries', href: '/industry-automotive' },
      { name: 'Healthcare & Medical', href: '/healthcaremedical-translation' },
      { name: 'Financial', href: '/financial-translation-services' },
      { name: 'Engineering & Technical', href: '/engineering-technical-translation' },
      { name: 'Legal', href: '/legal-translation-services' },
      { name: 'Gaming Website', href: '/industry-gaming' },
      { name: 'E-learning and Training', href: '/industry-elearning' }
    ]
  },
  { name: 'CAREERS', href: '/careers' },
  { name: 'BLOG', href: '/blog' },
  { name: 'CONTACT US', href: '/contact-us' }
]

const handleSearch = () => {
  if (searchQuery.value.trim()) {
    navigateTo(`/search?q=${encodeURIComponent(searchQuery.value)}`)
  }
}

const showDropdown = (menuName) => {
  if (dropdownTimeout.value) {
    clearTimeout(dropdownTimeout.value)
    dropdownTimeout.value = null
  }
  activeDropdown.value = menuName
}

const hideDropdown = () => {
  dropdownTimeout.value = setTimeout(() => {
    activeDropdown.value = ''
  }, 150) // Increased timeout to prevent premature closing
}

const keepDropdownOpen = () => {
  if (dropdownTimeout.value) {
    clearTimeout(dropdownTimeout.value)
    dropdownTimeout.value = null
  }
}

const toggleDropdown = (menuName) => {
  if (activeDropdown.value === menuName) {
    activeDropdown.value = ''
  } else {
    activeDropdown.value = menuName
  }
}

// Handle child navigation with proper dropdown closing
const handleChildNavigation = async (href) => {
  // Close dropdown immediately
  activeDropdown.value = ''
  // Clear any pending timeouts
  if (dropdownTimeout.value) {
    clearTimeout(dropdownTimeout.value)
    dropdownTimeout.value = null
  }
  // Navigate to the page
  try {
    await navigateTo(href)
  } catch (error) {
    console.error('Navigation error:', error)
    // Fallback: try with window.location if navigateTo fails
    window.location.href = href
  }
}

// Handle mobile navigation
const handleMobileParentNavigation = (item) => {
  if (!item.children) {
    mobileMenuOpen.value = false
  }
  // Let the NuxtLink handle the navigation
}

const handleMobileChildNavigation = async (href) => {
  mobileMenuOpen.value = false
  expandedMobileMenus.value = []

  try {
    await navigateTo(href)
  } catch (error) {
    console.error('Mobile navigation error:', error)
    // Fallback: try with window.location if navigateTo fails
    window.location.href = href
  }
}

const handleClickOutside = (event) => {
  const nav = event.target.closest('nav')
  const dropdown = event.target.closest('.relative.group')
  if (!nav && !dropdown) {
    activeDropdown.value = ''
  }
}

const toggleMobileSubmenu = (menuName) => {
  const index = expandedMobileMenus.value.indexOf(menuName)
  if (index > -1) {
    expandedMobileMenus.value.splice(index, 1)
  } else {
    expandedMobileMenus.value.push(menuName)
  }
}

// Close mobile menu when route changes
watch(() => useRoute().path, () => {
  mobileMenuOpen.value = false
  expandedMobileMenus.value = []
  activeDropdown.value = ''
})

onMounted(() => {
  document.addEventListener('click', handleClickOutside)
})

onUnmounted(() => {
  document.removeEventListener('click', handleClickOutside)
  if (dropdownTimeout.value) {
    clearTimeout(dropdownTimeout.value)
  }
})
</script>