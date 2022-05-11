<template>
  <div>
    <NavBar />
    <SearchArea />
    <div v-for="i in [1, 2, 3, 4, 5, 6, 7]" :key="i">
      <CardItem :key="i" />
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
