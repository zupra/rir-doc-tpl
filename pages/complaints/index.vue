<template>


<main class="xl:container mx-auto px-8">

  <header class="text-titanic flex justify-between">
    <div class="w-1/2">
      <h1 class="cheddar mb-4">Обращения</h1>
      <p class="parmigiano">Вместе мы сможем сделать наш город лучше! Следите за ходом и результатами работ по обращениям, которые подают жители города и области. </p>
    </div>
    <div class="flex">
      <div>
        <div class="cheddar text-rocky">128</div>
        <div class="mozzarella opacity-64">
          Обращения </br>подано
        </div>
      </div>
      <div class="ml-16">
        <div class="cheddar text-rocky">120</div>
        <div class="mozzarella opacity-64">
          Обращений </br>исполнено
        </div>
      </div>
    </div>
  </header>


  <img class="mt-12 mb-8 w-full shadow-lg rounded-3xl " src="https://static-maps.yandex.ru/1.x/?ll=37.677751,55.757718&spn=0.016457,0.00619&l=map&size=650,200" alt="">


  <div class="flex flex-wrap gap-8">

    <N-link to="/complaints/item" class="Card w-1/4 h-1/2 flex-shrink flex-grow shadow-lg rounded-3xl overflow-hidden"
      v-for="It in 15"
      :key="It.id"
    >
      <figure class="Card__content p-4 h-24 flex flex-col justify-between  text-white">
        <div class="flex flex-wrap">
          <div class="mozzarella px-3 py-1 bg-snatch rounded-full">
            Дворовые территории
          </div>
        </div>

        <figcaption>
          <h3 class="taleggio">Охранные зоны объектов электросетевого хозяйства.</h3>
          <p class="antialiased opacity-72">г. Волгодонск, Раменский р-он</p>
          <div class="flex mt-2">
            <img src="https://icongr.am/material/eye-outline.svg?size=24&color=315cb2" alt="">
            <div class="ml-2 opacity-72">12</div>
          </div>
        </figcaption>
      </figure>

      <picture class="">
        <img
          class="" 
          :src="`https://picsum.photos/id/${It+500}/480/320`" alt="">
      </picture>

    </N-link>
  </div>

</main>


</template>

<script>
export default {

}
</script>

<style scoped>

.Card {
  position: relative;
}

.Card:hover picture img {
  transform: scale(1.5);
  /* mask-image: linear-gradient(360deg, rgba(4, 21, 62, 0.8) 0%, rgba(4, 21, 62, 0) 90%); */
  /* mask-image: linear-gradient(rgba(0, 0, 0, .5), transparent); */
}

.Card__content {
  position: absolute;
  z-index: 1;
  height: 100%;
}

picture {
  position:relative;
  display:block;
  height: 100%;
}

picture:after {
  content:'';
  position:absolute;
  left:0; top:0;
  /* bottom: 0; */
  height:100%;
  width:100%; 
  background: linear-gradient(1turn, rgba(4, 21, 62, 0.8) 0%, rgba(4, 21, 62, 0) 100%);
}

picture img {
  height: 100%;
  width: 100%;
  object-fit: cover;
  transition: all .5s;
}
</style>