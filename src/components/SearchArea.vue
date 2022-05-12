<template>
  <div class="mx-10 my-5">
    <div class="mb-5">
      <h3 class="text-gray-900 font-semibold lg:text-2xl">
        Let’s find you a doctor
      </h3>
    </div>
    <div class="lg:flex lg:items-center lg:justify-around">
      <div class="flex items-center justify-center">
        <input
          type="text"
          placeholder="Search"
          class="bg-gray-200 w-80 h-14 rounded-xl"
        />
      </div>
      <div>
        <select
          class="invisible lg:visible border border-gray-100 rounded-lg w-[206px] h-[58px] bg-gray-200"
        >
          <option value="Location">Location</option>
        </select>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SearchArea',
}
</script>
