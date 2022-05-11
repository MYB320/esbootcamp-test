<template>
  <div>
    <NavBar />
    <DetailCard />
    <div class="flex justify-center items-center">
      <button class="w-[348px] h-[57px] bg-cyan-700 rounded-full text-white">
        Confirmer
      </button>
    </div>
  </div>
</template>

<script>
import NavBar from '@/components/NavBar'
import DetailCard from '@/components/DetailCard'
export default {
  name: 'DetailsView',
  components: { NavBar, DetailCard },
}
</script>
