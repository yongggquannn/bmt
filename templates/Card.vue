<template>
  <div>
    <div class="w-[300px] mr-[24px] shadow-xl rounded-xl overflow-hidden">
      <div class="h-[180px] bg-[#D3D8DE] text-center">
        <h3 class="text-2xl pt-[60px] px-5 font-bold"></h3>
      </div>

      <!-- ############# PART 3: HINT.. You'll need this! ############# -->
      <!-- <div class="h-[180px]">
        <img
          class="h-[180px] w-full"
          :src="require(`~assets/images/${item.image}.png`)"
        />
      </div> -->
      <!-- ############################################################ -->

      <div class="p-[20px]">
        <h3 class="mb-5 font-bold"></h3>
        <p class="mb-5"></p>
        <button class="bg-[#6245F4] text-white p-3 rounded-xl">
          Find out more
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CardDefault',

  // Hint: Add props here!
}
</script>
