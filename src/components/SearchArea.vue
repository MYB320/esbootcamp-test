<template>
  <div class="mx-10 my-5">
    <div class="mb-5">
      <h3 class="text-gray-900 font-semibold">Let’s find you a doctor</h3>
    </div>
    <div class="flex items-center justify-center">
      <input
        type="text"
        placeholder="   Search"
        class="bg-gray-100 w-80 h-14 rounded-xl"
      />
    </div>
    <div class="invisible">
      <select>
        <option value="Location">Location</option>
      </select>
    </div>
  </div>
</template>

<script>
export default {
  name: 'SearchArea',
}
</script>
