<template>
  <div>
    <NavBar />
    <div class="mx-10 my-5">
      <h3 class="text-gray-900 font-semibold text-xl">
        Take an appointment with
      </h3>
    </div>
    <CardItem />
    <CalendItem />
    <div class="flex justify-center items-center">
      <button class="w-[348px] h-[57px] bg-cyan-700 rounded-full text-white">
        Prendre rendez-vous
      </button>
    </div>
  </div>
</template>

<script>
import NavBar from '@/components/NavBar'
import CardItem from '@/components/CardItem'
import CalendItem from '@/components/CalendItem'
export default {
  name: 'BookingView',
  components: { NavBar, CardItem, CalendItem },
}
</script>
