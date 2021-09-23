<template>


<main class="container mx-auto px-8">

  <header class="text-titanic flex justify-between">
    <div class="w-1/2">
      <h1 class="cheddar mb-4">Голосования</h1>
      <p class="parmigiano">На голосования выносятся только вопросы, касающиеся граждан города и относящиеся к компетенции Правительства и органов исполнительной власти города или области.</p>
    </div>
    <div class="flex">
      <div>
        <div class="cheddar text-rocky">284</div>
        <div class="mozzarella opacity-64">
          Завершено
        </div>
      </div>
      <div class="ml-16">
        <div class="cheddar text-rocky">13437</div>
        <div class="mozzarella opacity-64">
          Открыто
        </div>
      </div>
    </div>
  </header>


  <div class="mt-12 flex flex-wrap gap-8">

    <N-link to="/votings/item" class="Voting bg-rush p-5 w-1/4 flex-shrink flex-grow shadow-sm hover:shadow-lg rounded-3xl overflow-hidden text-titanic"
      v-for="It in 15"
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

.Voting {
  display: grid;
  grid-template-rows: 5rem 3rem 24px;
}

</style>