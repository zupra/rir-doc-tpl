<template>

<div class="">

  <div class="max-w-6xl mx-auto">
    <transition
      enter-active-class="transition-opacity ease-linear duration-300"
      enter-class="opacity-0"
      enter-to-class="opacity-100"
      leave-active-class="transition-opacity ease-linear duration-300"
      leave-class="opacity-100"
      leave-to-class="opacity-0"
    >
      <MobileMenu v-show="showMobileMenu" @closeMobileMenu="showMobileMenu = false" />
    </transition>
    <MainHeader @showMobileMenu="showMobileMenu = true" v-show="!showMobileMenu" />
    <div class="flex">
      <DesktopSidebar class="hidden md:flex" />
      <Nuxt class="mt-24 px-6" />
    </div>
  </div>


  <footer class="text-gray-600 body-font  bg-blue-800">
    <div class="container px-5 py-24 mx-auto flex md:items-center lg:items-start md:flex-row md:flex-nowrap flex-wrap flex-col">
      <div class="w-64 flex-shrink-0 md:mx-0 mx-auto text-center md:text-left">
        <img src="https://test.rosatom.city/images-svg/rir_b8e179.svg" alt="">
      </div>
      <div class="flex-grow flex flex-wrap md:pl-20 -mb-10 md:mt-0 mt-10 md:text-left text-center">
        <div class="lg:w-1/4 md:w-1/2 w-full px-4">
          <h2 class=" burrata text-white mb-3">Категория</h2>
          <nav class="list-none mb-10">
            <li v-for="(link, idx) in 4" :key="idx">
              <a class="text-white hover:text-red-300" href="#">Ссылка</a>
            </li>
          </nav>
        </div>
        <div class="lg:w-1/4 md:w-1/2 w-full px-4">
          <h2 class=" burrata  text-white mb-3">Категория</h2>
          <nav class="list-none mb-10">
            <li v-for="(link, idx) in 4" :key="idx">
              <a class="text-white hover:text-red-300" href="#">Ссылка</a>
            </li>
          </nav>
        </div>
        <div class="lg:w-1/4 md:w-1/2 w-full px-4">
          <h2 class=" burrata  text-white mb-3">Категория</h2>
          <nav class="list-none mb-10">
            <li v-for="(link, idx) in 4" :key="idx">
              <a class="text-white hover:text-red-300" href="#">Ссылка</a>
            </li>
          </nav>
        </div>
        <div class="lg:w-1/4 md:w-1/2 w-full px-4">
          <h2 class=" burrata  text-white mb-3">Категория</h2>
          <nav class="list-none mb-10">
            <li v-for="(link, idx) in 4" :key="idx">
              <a class="text-white hover:text-red-300" href="#">Ссылка</a>
            </li>
          </nav>
        </div>
      </div>
    </div>
    <div class="bg-gray-900">
      <div class="container mx-auto py-4 px-5 flex flex-wrap flex-col sm:flex-row">
        <p class="text-white text-sm text-center sm:text-left">© 2021 Dev —
          <a href="https://wa.me/79261039948?text=from%20DOC" rel="noopener noreferrer" class="text-gray-400 ml-1" target="_blank">@Zupra</a>
        </p>
        <span class="inline-flex sm:ml-auto sm:mt-0 mt-2 justify-center sm:justify-start">
          <a class="text-gray-200">
            <svg fill="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" class="w-5 h-5" viewBox="0 0 24 24">
              <path d="M18 2h-3a5 5 0 00-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 011-1h3z"></path>
            </svg>
          </a>
          <a class="ml-3 text-gray-200">
            <svg fill="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" class="w-5 h-5" viewBox="0 0 24 24">
              <path d="M23 3a10.9 10.9 0 01-3.14 1.53 4.48 4.48 0 00-7.86 3v1A10.66 10.66 0 013 4s-4 9 5 13a11.64 11.64 0 01-7 2c9 5 20 0 20-11.5a4.5 4.5 0 00-.08-.83A7.72 7.72 0 0023 3z"></path>
            </svg>
          </a>
          <a class="ml-3 text-gray-200">
            <svg fill="none" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" class="w-5 h-5" viewBox="0 0 24 24">
              <rect width="20" height="20" x="2" y="2" rx="5" ry="5"></rect>
              <path d="M16 11.37A4 4 0 1112.63 8 4 4 0 0116 11.37zm1.5-4.87h.01"></path>
            </svg>
          </a>
          <a class="ml-3 text-gray-200">
            <svg fill="currentColor" stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="0" class="w-5 h-5" viewBox="0 0 24 24">
              <path stroke="none" d="M16 8a6 6 0 016 6v7h-4v-7a2 2 0 00-2-2 2 2 0 00-2 2v7h-4v-7a6 6 0 016-6zM2 9h4v12H2z"></path>
              <circle cx="4" cy="4" r="2" stroke="none"></circle>
            </svg>
          </a>
        </span>
      </div>
    </div>
  </footer>
</div>
</template>

<script>
export default {
  transition: {
    name: 'page',
    mode: 'out-in'
  },
  watch: {
    '$route' () {
      this.showMobileMenu = false
    }
  },
  data () {
    return {
      showMobileMenu: false
    }
  }
}
</script>

<style>
  /* .prose code {
    color: orange;
  }
  .prose a {
    color: #2563EB;
    text-decoration: none;
  }

  .prose a:hover {
    color: #3B82F6;
    text-decoration: none;
  } */
</style>
