<!-- ##### FOR TESTING! WON'T BE INCLUDED DURING LESSON -->
<template>
  <div>
    <div class="w-[300px] mr-[24px] shadow-xl rounded-xl overflow-hidden">
      <!-- PART 3: VUE DIRECTIVES!! -->

      <!-- <div v-if="item.image === ''" class="h-[180px] bg-[#D3D8DE] text-center">
        <h3 class="text-2xl pt-[60px] px-5 font-bold">{{ item.title1 }}</h3>
      </div>
      <div v-else> -->
      <!-- NEED TO REWORK IMG CODE, IMG DOESN'T APPEAR -->
      <!-- <img class="" :src="item.image" />
      </div> -->

      <div class="h-[180px] bg-[#D3D8DE] text-center">
        <h3 class="text-2xl pt-[60px] px-5 font-bold">{{ item.title1 }}</h3>
      </div>
      <div class="p-[20px]">
        <h3 class="mb-5 font-bold">{{ item.title2 }}</h3>
        <p class="mb-5">{{ item.description }}</p>
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
  // methods: {
  //   header(color) {
  //     let stylename = 'background-color: '
  //     stylename += color
  //     return stylename
  //   },
  // },
  props: {
    item: {
      type: Object,
      required: true,
    },
  },
}
</script>
