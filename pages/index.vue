<template>

<div class="container mx-auto">



  <h2 class="text-2xl font-semibold">
    Библиотеки
  </h2>
  <div class="bg-white w-full min-w-3xl overflow-x-scroll shadow-md rounded my-6">
    <table class="text-left w-full border-collapse">
      <thead>
      <tr>
        <th class="py-4 px-6 bg-grey-lightest font-bold uppercase text-sm text-grey-dark border-b border-grey-light">Библиотека</th>
        <th class="py-4 px-6 bg-grey-lightest font-bold uppercase text-sm text-grey-dark border-b border-grey-light">Description</th>
      </tr>
      </thead>
      <tbody>
      <tr class="hover:bg-grey-lighter">
        <td class="py-4 px-6 border-b border-grey-light">
          <a href="https://vitejs.dev/guide/" class="text-blue-500 hover:text-blue-700" target="_blank">
            vite
          </a>
        </td>
        
        <td class="py-4 px-6 border-b border-grey-light text-sm">
          Vite вместо Webpack во время разработки
        </td>
      </tr>

      <tr class="hover:bg-grey-lighter">
        <td class="py-4 px-6 border-b border-grey-light">
          <a href="https://windicss.org/guide/" class="text-blue-500 hover:text-blue-700" target="_blank">
            windicss
          </a>
        </td>
        
        <td class="py-4 px-6 border-b border-grey-light text-sm">
          альтернатива Tailwind, которая обеспечивает более быстрое время загрузки, полностью совместима с Tailwind v2.0 и имеет множество дополнительных интересных функций
        </td>
      </tr>

      <tr class="hover:bg-grey-lighter">
        <td class="py-4 px-6 border-b border-grey-light">
          <a href="https://content.nuxtjs.org" class="text-blue-500 hover:text-blue-700" target="_blank">
            @nuxt/content
          </a>
        </td>

        <td class="py-4 px-6 border-b border-grey-light text-sm">
          Create blogs and docs using markdown and Vue components 
          <a href="https://nuxtjs.org/tutorials/creating-blog-with-nuxt-content/" class="text-blue-500 hover:text-blue-700">Описание</a>
        </td>
      </tr>
      <tr class="hover:bg-grey-lighter">
        <td class="py-4 px-6 border-b border-grey-light">
          <a href="https://github.com/drdogbot7/tailwindcss-responsive-embed" class="text-blue-500 hover:text-blue-700" target="_blank">
            tailwindcss-responsive-embed
          </a>
        </td>
        <td class="py-4 px-6 border-b border-grey-light text-sm">
          Make embedded content responsive
        </td>
      </tr>
      <tr class="hover:bg-grey-lighter">
        <td class="py-4 px-6 border-b border-grey-light">
          <a href="https://github.com/tailwindlabs/tailwindcss-aspect-ratio" class="text-blue-500 hover:text-blue-700" target="_blank">
            tailwindcss-aspect-ratio
          </a>
        </td>
        <td class="py-4 px-6 border-b border-grey-light text-sm">
          Display ideal aspect rations for media
        </td>
      </tr>
      <tr class="hover:bg-grey-lighter">
        <td class="py-4 px-6 border-b border-grey-light">
          <a href="https://tailwindcss.com/docs/typography-plugin" class="text-blue-500 hover:text-blue-700" target="_blank">
            @tailwindcss/typography
          </a>
        </td>
        <td class="py-4 px-6 border-b border-grey-light text-sm">
          Style html converted from Markdown with Prose class
        </td>
      </tr>
      <tr class="hover:bg-grey-lighter">
        <td class="py-4 px-6 border-b border-grey-light">
          <a href="https://www.npmjs.com/package/nuxt-content-algolia" class="text-blue-500 hover:text-blue-700" target="_blank">
            nuxt-content-algolia
          </a>
        </td>
        <td class="py-4 px-6 border-b border-grey-light text-sm">
          Deliver documentation content to your Algolia indices
        </td>
      </tr>
      <tr class="hover:bg-grey-lighter">
        <td class="py-4 px-6 border-b border-grey-light">
          <a href="https://www.algolia.com/doc/guides/building-search-ui/what-is-instantsearch/vue/" class="text-blue-500 hover:text-blue-700" target="_blank">
            vue-instantsearch
          </a>
        </td>
        <td class="py-4 px-6 border-b border-grey-light text-sm">
          Algolia search components made for VueJS
        </td>
      </tr>
      <tr class="hover:bg-grey-lighter">
        <td class="py-4 px-6 border-b border-grey-light">
          <a href="https://www.npmjs.com/package/v-click-outside" class="text-blue-500 hover:text-blue-700" target="_blank">
            v-click-outside
          </a>
        </td>
        <td class="py-4 px-6 border-b border-grey-light text-sm">
          Detect outside clicks - great for collapsing dropdown menus
        </td>
      </tr>
      </tbody>
    </table>
  </div>



  <!-- <pre class="h-60 overflow-y-auto text-xs bg-gray-200 p-4">{{defineConfig()}}</pre> -->


</div>
</template>

<script>
// import {theme} from '~/windi.config.ts'

export default {
  data() {
    return {
      // windiConfig,
      // theme,
    };
  }
}
</script>

<style>
</style>
