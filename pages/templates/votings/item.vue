<template>

<main class="xl:container mx-auto px-8">
  <section class="w-620px mx-auto">

    <N-link to="/templates/votings" class="parmigiano opacity-72 hover:text-blue-600">
      / Голосования
    </N-link>

    <h1 class="cheddar my-4">Нужны ли электробусы на городских улицах?</h1>

    <div class="parmigiano opacity-72 flex items-center">
      <CIconBase color="#3D75E4">
        <path d="M4.5 1c0-.552285.44772-1 1-1h5c.5523 0 1 .447715 1 1 0 .55228-.4477 1-1 1H9v1.07645c3.1151.481 5.5 3.17376 5.5 6.42355 0 3.5899-2.9101 6.5-6.5 6.5-3.58985 0-6.5-2.9101-6.5-6.5 0-2.12723 1.0231-4.01543 2.59939-5.19954.44157-.33171 1.06844-.24265 1.40015.19893.33171.44157.24265 1.06844-.19893 1.40015C4.20534 6.72231 3.5 8.02861 3.5 9.5 3.5 11.9853 5.51472 14 8 14c2.4853 0 4.5-2.0147 4.5-4.5C12.5 7.01472 10.4853 5 8 5c-.55228 0-1-.44772-1-1V2H5.5c-.55228 0-1-.44772-1-1Z" />
        <path d="M8.98189 7.16442c.867.30017 1.55361.98675 1.85371 1.85374.1807.52189-.2833.98194-.8356.98194H9c-.55228 0-1-.44776-1-1.00005v-1c0-.55228.46-1.01631.98189-.83563Z" />
      </CIconBase>
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
          <CIconBase color="#3D75E4">
            <path d="M4.5 1c0-.552285.44772-1 1-1h5c.5523 0 1 .447715 1 1 0 .55228-.4477 1-1 1H9v1.07645c3.1151.481 5.5 3.17376 5.5 6.42355 0 3.5899-2.9101 6.5-6.5 6.5-3.58985 0-6.5-2.9101-6.5-6.5 0-2.12723 1.0231-4.01543 2.59939-5.19954.44157-.33171 1.06844-.24265 1.40015.19893.33171.44157.24265 1.06844-.19893 1.40015C4.20534 6.72231 3.5 8.02861 3.5 9.5 3.5 11.9853 5.51472 14 8 14c2.4853 0 4.5-2.0147 4.5-4.5C12.5 7.01472 10.4853 5 8 5c-.55228 0-1-.44772-1-1V2H5.5c-.55228 0-1-.44772-1-1Z" />
            <path d="M8.98189 7.16442c.867.30017 1.55361.98675 1.85371 1.85374.1807.52189-.2833.98194-.8356.98194H9c-.55228 0-1-.44776-1-1.00005v-1c0-.55228.46-1.01631.98189-.83563Z" />
          </CIconBase>
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