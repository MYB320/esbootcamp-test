<template>
  <div>
    <NavBar />
    <SearchArea />
    <div>
      <dir>
        <h3 class="text-gray-900 font-semibold text-xl my-8 mx-10">À la une</h3>
        <div class="grid lg:grid-cols-4 lg:gap-1">
          <div v-for="i in [1, 2, 3, 4]" :key="i">
            <MoreDetails />
          </div>
        </div>
      </dir>
      <div>
        <h3 class="text-gray-900 font-semibold text-xl my-8 mx-10">
          Recommended
        </h3>
        <div class="grid lg:grid-cols-3 lg:gap-1">
          <div v-for="i in [1, 2, 3, 4, 5, 6, 7]" :key="i">
            <CardItem />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import NavBar from '@/components/NavBar'
import SearchArea from '@/components/SearchArea'
import CardItem from '@/components/CardItem'
import MoreDetails from '@/components/MoreDetails'
export default {
  name: 'HomeView',
  components: { NavBar, SearchArea, CardItem, MoreDetails },
}
</script>
