<template>

<div class="container w-full">

  <h2 class="text-2xl font-semibold">
    Libraries Used
  </h2>
  <div class="bg-white w-full min-w-3xl overflow-x-scroll shadow-md rounded my-6">
    <table class="text-left w-full border-collapse">
      <thead>
      <tr>
        <th class="py-4 px-6 bg-grey-lightest font-bold uppercase text-sm text-grey-dark border-b border-grey-light">Library</th>
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







  <div class="prose">

    <h1 class="!mb-8 !mt-12">Палитра</h1>

    <p>Палитра состоит из шести цветов с девятью оттенками в каждом. Основным фирменным цветом является синий. Он всегда используется в первую очередь. Оттенки серого используются для оформления тёмной темы интерфейса.</p>

    <p>Остальные цвета могут использоваться для цветового кодирования, а оттенки красного и зелёного также в сообщениях об ошибах и «успехах».</p>


    <p>Тёмные оттенки используются для оформления текстов, 5-й — кнопок и прочих интерактивных элементов, а светлые — плашек и фонов.</p>

    <div class="row_2">
      <div class="col" v-for="(chunk, idx) in colors_9_chunk" :key="idx">
        <div class="cell sb" v-for="(color, name, index) in chunk" :key="index" :style="{ backgroundColor: color }"><small :style="{ color: index % 9 &gt; 4 ? '#444' : '#EEE' }">{{ name }}</small>
          <div :style="{ color: index % 9 &gt; 4 ? '#444' : '#CCC' }">{{ color }}</div>
        </div>
      </div>
    </div>


    <h1 class="!mb-8 !mt-12">Заголовки</h1>
    <div class="grid">
      <div class="fontItem" v-for="(V, K, idx) in headerFonts" :key="idx">
        <div class="view text-godfather" :class="K">.{{ K }}</div>
        <pre class=" !overflow-x-visible">{{ V }}</pre>
      </div>
    </div>
    <h1 class="!mb-8 !mt-12">Основной наборный текст</h1>
    <div class="grid">
      <div class="fontItem" v-for="(V, K, idx) in basicFonts" :key="idx">
        <div class="view" :style="V" :class="K">.{{ K }}</div>
        <pre class=" !overflow-x-visible">{{ V }}</pre>
      </div>
    </div>
    <h1 class="!mb-8 !mt-12">Дополнительный текст</h1>
    <div class="grid">
      <div class="fontItem" v-for="(V, K, idx) in additionalFonts" :key="idx">
        <div class="view" :style="V" :class="K">.{{ K }}</div>
        <pre class=" !overflow-x-visible">{{ V }}</pre>
      </div>
    </div>
    <h1 class="!mb-8 !mt-12">Контролы</h1>
    <div class="grid">
      <div class="fontItem" v-for="(V, K, idx) in controlsFonts" :key="idx">
        <div class="view" :style="V" :class="K">.{{ K }}</div>
        <pre class=" !overflow-x-visible">{{ V }}</pre>
      </div>
    </div>
  </div>


  <!-- <pre class="h-60 overflow-y-auto text-xs bg-gray-200 p-4">{{tailwindConfig}}</pre> -->

  <!-- This is the landing page content - swap out with your own -->




</div>
</template>

<script>
// import tailwindConfig from '~/tailwind.config'



const headerFonts = {
  primo: {
    'font-size': '72px',
    'line-height': '72px',
    'font-weight': '700',
  },
  gouda: {
    'font-size': '56px',
    'line-height': '56px',
    'font-weight': '700',
  },
  cheddar: {
    'font-size': '40px',
    'line-height': '44px',
    'font-weight': '700',
  },
  camembert: {
    'font-size': '32px',
    'line-height': '36px',
    'font-weight': '700',
  },
  ricotta: {
    'font-size': '28px',
    'line-height': '32px',
    'font-weight': '700',
  },
  burrata: {
    'font-size': '24px',
    'line-height': '28px',
    'font-weight': '700',
  },
  taleggio: {
    'font-size': '20px',
    'line-height': '24px',
    'font-weight': '700',
  },
  comte: {
    'font-size': '20px',
    'line-height': '28px',
    'font-weight': '700',
  },
  bryndza: {
    'font-size': '16px',
    'line-height': '20px',
    'font-weight': '700',
  },
  tulum: {
    'font-size': '16px',
    'line-height': '24px',
    'font-weight': '700',
  }
};

const basicFonts = {
  mascarpone: {
    'font-size': '20px',
    'line-height': '28px',
    'font-weight': '400',
  },
  brie: {
    'font-size': '20px',
    'line-height': '24px',
    'font-weight': '400',
  },
  parmigiano: {
    'font-size': '16px',
    'line-height': '24px',
    'font-weight': '400',
  },
  feta: {
    'font-size': '16px',
    'line-height': '20px',
    'font-weight': '400',
  }
}; 


const additionalFonts = {  
  mozzarella: {
    'font-size': '13px',
    'line-height': '16px',
    'font-weight': '400',
  },
  roquefort: {
    'font-size': '13px',
    'line-height': '16px',
    'font-weight': '700',
  },
  сaprino: {
    'font-size': '10px',
    'line-height': '12px',
    'font-weight': '400',
  }
};

const controlsFonts = { 
  maasdam: {
    'font-size': '20px',
    'line-height': '24px',
    'font-weight': '500',
  },
  sulguni: {
    'font-size': '16px',
    'line-height': '20px',
    'font-weight': '500',
  },
  briscola: {
    'font-size': '13px',
    'line-height': '16px',
    'font-weight': '500',
  },
  edam: {
    'font-size': '10px',
    'line-height': '12px',
    'font-weight': '500',
  }
};



const colors = {
  titanic: '#04153E',
  gladiator: '#091F52',
  interstellar: '#113079',
  godfather: '#214EB0',
  rocky: '#3D75E4',
  alien: '#81ABEE',
  memento: '#C0D6F6',
  arrival: '#E4EDFB',
  rush: '#F6F9FE',
  bladerunner: '#111827',
  harakiri: '#1C2331',
  vertigo: '#2E3648',
  troy: '#495469',
  metropolis: '#6F7A90',
  pianist: '#A2ABBE',
  inception: '#CDD3DF',
  apocalypse: '#E6EBF5',
  trainspotting: '#F5F8FC',
  extraction: '#21043E',
  room: '#300F52',
  heat: '#4A197B',
  casino: '#6D3AA6',
  gentlemen: '#9954F2',
  seven: '#BB9AF4',
  unforgiven: '#DBCCFA',
  departed: '#EFE8FC',
  intouchables: '#F9F6FE',
  prestige: '#34040F',
  exorcist: '#480A17',
  predator: '#711426',
  stalker: '#AB213A',
  fargo: '#E14761',
  indiana: '#F196A5',
  bandit: '#F7CFD5',
  romance: '#FBE9EC',
  joker: '#FEF8F9',
  oldBoy: '#142202',
  forest: '#1F3404',
  whiplash: '#304D0A',
  shining: '#467510',
  matrix: '#57A003',
  drive: '#8DC95E',
  psycho: '#C7E6A8',
  amadeus: '#E3F3D8',
  shawshank: '#F6FCF3',
  schindler: '#2A1704',
  capernaum: '#3A1F03',
  platoon: '#643302',
  mulHolland: '#9E4F00',
  lebowski: '#D06E0B',
  snatch: '#E9A35D',
  chinatown: '#F8D6B5',
  jaws: '#FBECDD',
  warrior: '#FEFAF6',
}

export default {
  data() {
    return {
      // tailwindConfig,
      headerFonts,
      basicFonts,
      additionalFonts,
      controlsFonts,
      colors,
    };
  },
  computed: {
    colors_9_chunk() {
      let myArray = Object.entries(this.colors);
      let results = [];
      while (myArray.length) {
        results.push(
          myArray.splice(0, 9).reduce(
            (acc, curr) => ({
              ...acc,
              [curr[0]]: curr[1],
            }),
            {},
          ),
        );
      }
      return results;
    },
  },
}
</script>

<style>


.row_2 {
  display: grid;
  /* grid-template-columns: repeat(6, 180px); */
  grid-template-columns: repeat(6, 1fr);
}
.col {
  display: flex;
  flex-direction: column;
}


.cell {
  padding: .5em;
}
/* .sb {
  display: flex;
  justify-content: space-between;
} */

/* ++++++++ */

.grid {
  margin: 2em 0;
  display: grid;
  grid-template-columns: min-content min-content;
  gap: 30px;
}

.fontItem {
  display: grid;
  grid-template-columns: auto 1fr;
  align-items: baseline;
  border-bottom: 1px solid #ccc;
}

.view {
  color: #3D75E4;
}


</style>
