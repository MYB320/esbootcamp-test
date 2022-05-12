<template>
  <div
    id="defaultModal"
    tabindex="-1"
    aria-hidden="true"
    class="hidden overflow-y-auto overflow-x-hidden fixed top-0 right-0 left-0 z-50 w-full md:inset-0 h-modal md:h-full"
  >
    <div class="relative p-4 w-full max-w-2xl h-full md:h-auto">
      <!-- Modal content -->
      <div class="relative bg-white rounded-lg shadow dark:bg-gray-700">
        <div class="mx-10 my-5">
          <h3 class="text-gray-900 font-semibold text-xl">
            Take an appointment with
          </h3>
        </div>
        <CardItem />
        <CalendItem />
        <div class="flex justify-center items-center">
          <button
            class="w-[348px] h-[57px] bg-cyan-700 rounded-full text-white"
          >
            Prendre rendez-vous
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import CardItem from '@/components/CardItem'
import CalendItem from '@/components/CalendItem'

export default {
  name: 'BookingPopup',
  components: { CardItem, CalendItem },
}
</script>

<style></style>
