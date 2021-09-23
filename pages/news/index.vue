<template>


<main class="xl:container mx-auto px-8">

  <h1 class="cheddar mb-14">Новости</h1>

  <div class="flex flex-wrap gap-8">

    <N-link to="/news/item" class="Card w-1/4 flex-shrink flex-grow"
      v-for="It in 15"
      :key="It.id"
    >
      <figure>
        <picture class="block aspect-9/16">
          <img
            class="shadow-lg rounded-3xl" 
            :src="`https://picsum.photos/id/${It+303}/480/320`" alt="">
        </picture>
        <figcaption>
          <h3 class="taleggio mt-4 mb-2">Репетиции парада Победы в Мурманске состоятся 5 и 7 мая</h3>
          <div class="parmigiano opacity-48">
            20 апреля
          </div>
        </figcaption>
      </figure>
    </N-link>
  </div>

</main>



</template>

<script>
export default {

}
</script>

<style>

</style>