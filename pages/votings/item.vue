<template>

<main class="xl:container mx-auto px-8">
  <section class="w-620px mx-auto">

    <N-link to="/votings" class="parmigiano opacity-72 hover:text-blue-600">
      / Голосования
    </N-link>

    <h1 class="cheddar my-4">Нужны ли электробусы на городских улицах?</h1>

    <div class="parmigiano opacity-72 flex">
      <img src="https://icongr.am/material/alarm.svg?size=16&color=315cb2" alt="">
      <div class="ml-1">Завершится 30 апреля, 16:00</div>
    </div>


    <picture class="block aspect-9/16 my-8">
      <img
        class="shadow-lg rounded-3xl" 
        :src="`https://picsum.photos/id/490/900/600`" alt="">
    </picture>


    <article class="parmigiano opacity-72">    
      <p class="mb-3">Дороги будущего покорит электробус. В перспективе именно этот вид наземного транспорта станет основным средством передвижения по городу, а дизельные автобусы уйдут в прошлое. Уже сейчас всё чаще совершают поездки на электробусах. На различных маршрутах курсирует уже больше 200 таких машин. За год электробусы преодолели в общей сложности 3,5 миллиона километров и перевезли 11 миллионов пассажиров.</p>
    </article>

    <div class="text-rocky flex font-medium mt-10 mb-16">
      <a href="#">Скачать презентацию</a>
    </div>
  </section>






  <div class="mt-12 flex flex-wrap gap-8">

    <N-link to="/votings/item" class="Voting bg-rush p-5 w-1/4 flex-shrink flex-grow shadow-sm hover:shadow-lg rounded-3xl overflow-hidden text-titanic"
      v-for="It in 3"
      :key="It.id"
    >
      <div class="bryndza">
        Организация зимних видов спорта и рекреационных зон на склонах
      </div>

      <div>
        <div class="mozzarella flex">
          <img src="https://icongr.am/material/alarm.svg?size=16&color=315cb2" alt="">
          <div class="ml-1">До 12 июля</div>
        </div>
      </div>

      <div class="flex">
        <div class="mozzarella px-4 py-1 bg-alien rounded-full text-white">
          Ремонтные работы
        </div>
      </div>
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