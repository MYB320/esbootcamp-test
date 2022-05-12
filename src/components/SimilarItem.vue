<template>
  <div class="bg-[#F9FAFB] border border-gray-100">
    <h3 class="text-gray-500 text-2xl text-center my-16 font-medium">
      Similars
    </h3>
    <div v-for="i in [1, 2, 3, 4, 5, 6, 7]" :key="i">
      <CardItem />
    </div>
  </div>
</template>

<script>
import CardItem from '@/components/CardItem'
export default {
  name: 'SimilarItem',
  components: { CardItem },
}
</script>
