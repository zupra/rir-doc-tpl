<template>

<div class="Sidebar flex flex-col p-4">
  <div class="flex">
    <img src="https://icongr.am/material/newspaper-variant-outline.svg?size=24&color=315cb2" alt="">
    <div class="ml-3 font-light tracking-wide text-gray-500">МАКЕТЫ</div>
  </div>

  <!-- Новости -->
  <div class="flex items-center my-3">
    <div class="flex items-center justify-center h-8 w-8 bg-indigo-200 rounded-full">H</div>
    <div class="ml-1 text-sm font-light tracking-wide text-gray-500">Новости</div>
  </div>
  <ol class="leading-none underline-green-500 list-square pl-5">
    <li>
      <N-link to="/news" 
        class="text-gray-600 hover:text-blue-500 group flex items-center pb-3">
        Новости (список)
      </N-link>
    </li>
    <li>
      <N-link to="/news/item" 
        class="text-gray-600 hover:text-blue-500 group flex items-center pb-3">
        Новости (страница новости)
      </N-link>
    </li>
  </ol>

  <!-- Обращения -->
  <div class="flex items-center my-3">
    <div class="flex items-center justify-center h-8 w-8 bg-orange-200 rounded-full">О</div>
    <div class="ml-1 text-sm font-light tracking-wide text-gray-500">Обращения</div>
  </div>
  <ol class="leading-none underline-green-500 list-square pl-5">
    <li>
      <N-link to="/complaints" 
        class="text-gray-600 hover:text-blue-500 group flex items-center pb-3">
        Обращения (список)
      </N-link>
    </li>
    <li>
      <N-link to="/complaints/item" 
        class="text-gray-600 hover:text-blue-500 group flex items-center pb-3">
        Обращения (страница обращения)
      </N-link>
    </li>
  </ol>

  <!-- Голосования -->
  <div class="flex items-center my-3">
    <div class="flex items-center justify-center h-8 w-8 bg-pink-200 rounded-full">Г</div>
    <div class="ml-1 text-sm font-light tracking-wide text-gray-500">Голосования</div>
  </div>
  <ol class="leading-none underline-green-500 list-square pl-5">
    <li>
      <N-link to="/votings" 
        class="text-gray-600 hover:text-blue-500 group flex items-center pb-3">
        Голосования (список)
      </N-link>
    </li>
    <li>
      <N-link to="/votings/item" 
        class="text-gray-600 hover:text-blue-500 group flex items-center pb-3">
        Голосования (страница голосования)
      </N-link>
    </li>
  </ol>




  <h3 class="bryndza uppercase text-gray-700 py-3">
    UI
  </h3>
  <N-link to="/UI/colors" 
  class="text-sm text-gray-500 hover:text-blue-500 group flex items-center pb-3 pl-3">
    ЦВЕТ
  </N-link>

  <N-link to="/UI/typography" 
  class="text-sm text-gray-500 hover:text-blue-500 group flex items-center pb-3 pl-3">
    Типографика
  </N-link>

  <N-link to="/UI/badge" 
  class="text-sm text-gray-500 hover:text-blue-500 group flex items-center pb-3 pl-3">
    badge
  </N-link>



  <h3 class="bryndza uppercase text-gray-700 py-3">
    Section
  </h3>
  <N-link to="/demo_5" 
  v-for="It in 10"
  :key="`5_${It}`"
  class="text-sm text-gray-500 hover:text-blue-500 group flex items-center pb-3 pl-3">
    Ссылка_{{It}}
  </N-link>

  <h3 class="bryndza uppercase text-gray-700 py-3">
    Section
  </h3>
  <N-link to="/demo_4" 
  v-for="It in 10"
  :key="`4_${It}`"
  class="text-sm text-gray-500 hover:text-blue-500 group flex items-center pb-3 pl-3">
    Ссылка_{{It}}
  </N-link>
</div>

</template>

<script>
export default {

}
</script>

<style>

.nuxt-link-active {

}
.Sidebar .nuxt-link-exact-active {
  @apply text-blue-500 font-bold;
}


</style>