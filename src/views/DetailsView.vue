<template>
  <div class="lg:grid lg:grid-cols-4">
    <div class="lg:col-span-3 order-2">
      <NavBar />
      <div class="lg:flex lg:justify-around">
        <DetailCard />
        <div class="flex justify-center items-center flex-col my-4 w-[348px]">
          <button
            class="w-[348px] h-[57px] bg-cyan-700 rounded-full text-white"
            type="button"
            data-modal-toggle="defaultModal"
          >
            Confirmer
          </button>

          <div
            class="invisible lg:visible order-3 mt-4 w-[348px]"
            v-for="i in [1, 2, 3, 4, 5]"
            :key="i"
          >
            <RatingItem />
          </div>
        </div>
      </div>
    </div>
    <div class="invisible lg:visible order-1"><SimilarItem /></div>
    <div class="invisible lg:visible order-4">
      <BookingPopup />
    </div>
  </div>
</template>

<script>
import NavBar from '@/components/NavBar'
import DetailCard from '@/components/DetailCard'
import SimilarItem from '@/components/SimilarItem'
import RatingItem from '@/components/RatingItem'
import BookingPopup from '@/components/BookingPopup'
export default {
  name: 'DetailsView',
  components: { NavBar, DetailCard, SimilarItem, RatingItem, BookingPopup },
}
</script>
