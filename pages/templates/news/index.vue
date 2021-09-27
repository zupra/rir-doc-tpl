<template>


<main class="container mx-auto px-8">


  <!-- <pre>{{News}}</pre> -->

  <h1 class="cheddar mb-14">Новости</h1>

  <div class="flex flex-wrap gap-8">

    <N-link to="/templates/news/item" class="group w-1/4 flex-shrink flex-grow"
      v-for="(It,idx) in News"
      :key="idx"
    >
      <!-- <picture class="block aspect-9/16">
        <img
          class="shadow-lg rounded-3xl" 
          :src="`https://picsum.photos/id/${It+303}/480/320`" alt=""
        >
      </picture>
      <h3 class="taleggio mt-4 mb-2 group-hover:text-interstellar">Репетиции парада Победы в Мурманске состоятся 5 и 7 мая</h3>
      <div class="parmigiano opacity-48 group-hover:opacity-64">20 апреля</div> -->

      
      <figure>
        <picture class="block aspect-9/16">
          <img
            class="shadow-lg rounded-16" 
            :src="`https://picsum.photos/id/${idx+304}/480/320`" alt="">
        </picture>
        <figcaption>
          <h3 class="line-clamp-3 taleggio mt-4 mb-2 group-hover:text-interstellar">{{It.title}}</h3>
          <div class="parmigiano opacity-48 group-hover:opacity-64">20 апреля</div>
        </figcaption>
      </figure>


      
    </N-link>

  </div>

</main>



</template>

<script>
import { News } from '~/mock_data'

export default {

  data() {
    return {
      News
    };
  },
}
</script>

<style>

</style>