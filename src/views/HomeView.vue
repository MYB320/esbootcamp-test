<template>
  <div>
    <NavBar />
    <SearchArea />
    <div class="grid lg:grid-cols-3 lg:gap-1">
      <div v-for="i in [1, 2, 3, 4, 5, 6, 7]" :key="i">
        <CardItem />
      </div>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import NavBar from '@/components/NavBar'
import SearchArea from '@/components/SearchArea'
import CardItem from '@/components/CardItem'
export default {
  name: 'HomeView',
  components: { NavBar, SearchArea, CardItem },
}
</script>
