<template>

<main class="xl:container mx-auto px-8">
  <section class="w-620px mx-auto">

    <N-link to="/templates/votings" class="parmigiano opacity-72 hover:text-blue-600">
      / Голосования
    </N-link>

    <h1 class="cheddar my-4">Нужны ли электробусы на городских улицах?</h1>

    <div class="parmigiano opacity-72 flex">
      <img src="https://icongr.am/material/alarm.svg?size=16&color=315cb2" alt="">
      <div class="ml-1">Завершится 30 апреля, 16:00</div>
    </div>


    <picture class="block aspect-9/16 my-8">
      <img
        class="shadow-lg rounded-16" 
        :src="`https://picsum.photos/id/490/900/600`" alt="">
    </picture>


    <article class="parmigiano opacity-72">    
      <p class="mb-3">Дороги будущего покорит электробус. В перспективе именно этот вид наземного транспорта станет основным средством передвижения по городу, а дизельные автобусы уйдут в прошлое. Уже сейчас всё чаще совершают поездки на электробусах. На различных маршрутах курсирует уже больше 200 таких машин. За год электробусы преодолели в общей сложности 3,5 миллиона километров и перевезли 11 миллионов пассажиров.</p>
    </article>


    <div class="flex gap-5 mt-2 mb-4 py-3 pl-6 bg-rose-50 rounded-16">
      <div
      v-for="(tab, idx) in ['Проголосовал', 'С картинкой', 'Текст +checkbox']" 
      :key="idx" 
      @click="TAB = idx+1"
      class="sulguni text-gray-500 cursor-pointer pb-1" 
      :class="idx === TAB-1 && 'text-gray-800 border-b-blue-500 border-b-4'" 
      >
      {{ tab }}
      </div>
    </div>
    <transition-group name="tab">
      <SECTION key="tab_1" v-show="TAB===1" class="flex flex-col gap-y-10">
        <div v-for="(It, idx) in [
          {
            title: 'Сноутубинг',
            percent: 23.4,
          },
          {
            title: 'Каток',
            percent: 19.6,
            color: 'green'
          },
          {
            title: 'Лыжи',
            percent: 12.7,
            color: 'green'
          },
          {
            title: 'Сноуборд',
            percent: 38.3,
          }
        ]" :key="idx">
          <C-Progress 
            :title="It.title"
            text="ул. Новоясеневская, 131"
            :percent="It.percent"
            :color="It.color"
          />
        </div>
      </SECTION>
      <SECTION key="tab_2" v-show="TAB===2" class="flex flex-col gap-y-10">
        <div class="flex items-center" v-for="(It, idx) in ['Сноутубинг','Каток','Лыжи','Сноуборд']" :key="idx">
          <input type="radio">

          <!-- 
          <picture class="mx-3 shadow-lg rounded-8 h-56px w-56px">
          </picture> 
          -->
          <img
          class="block mx-3 shadow-lg rounded-8"
            :src="`https://picsum.photos/id/${idx+30}/56/56`" alt="">

          <div>
            <div class="sulguni">
            {{It}}
            </div>
            <div class="briscola opacity-64">ул. Новоясеневская, 131</div>
          </div>
        </div>
      </SECTION>
      <SECTION key="tab_3" v-show="TAB===3" class="flex flex-col gap-y-5">
        <div class="flex items-baseline" v-for="(It, idx) in ['Сноутубинг','Каток','Лыжи','Сноуборд']" :key="idx">
          <input type="checkbox">
          <div class="ml-3">
            <div class="sulguni">
            {{It}}
            </div>
            <div class="briscola opacity-64">ул. Новоясеневская, 131</div>
          </div>
        </div>
      </SECTION>
    </transition-group>



    <div class="mt-10 text-rocky flex font-medium mb-16">
      <a href="#">Скачать презентацию</a>
    </div>
  </section>






  <div class="mt-12 flex flex-wrap gap-8">

    <N-link to="/templates/votings/item" class="Voting bg-rush p-5 w-1/4 flex-shrink flex-grow shadow-sm hover:shadow-lg rounded-3xl overflow-hidden"
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
data () {
    return {
      TAB: 1
    }
  }


}
</script>

<style>

.tab-enter-active {
  transition: all .4s ease
}
.tab-enter {
  opacity: 0;
  transform: translateY(10px)
}
.tab-enter-to {
  opacity: 1
}
.tab-leave-active {
  display: none
}

</style>