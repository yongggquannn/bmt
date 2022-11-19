<template>
  <div>
    <div
      class="flex bg-gradient-to-r from-[#FFE543] to-[#FFCD19] p-7 pl-10 mb-7"
    >
      <!-- ############# PART 1: PROJ STRUCTURE!! ############## -->
      <!-- ###      Add in HOGC Logo into assets folder,     ### -->
      <!-- ###      and add the file path in the img tag     ### -->
      <!-- ##################################################### -->

      <img class="mr-5" src="??" />
      <h3 class="text-2xl font-bold">HOGC One</h3>
    </div>
    <h1 class="text-3xl m-10 mb-4 font-bold">Happenings</h1>
    <p class="ml-10 mb-7">
      Stay in the know on the latest happenings & buzz in church!
    </p>

    <!-- ############# PART 2: PROPS & DATA!! ############## -->
    <!-- ###   Create your card using the 'item' below   ### -->
    <!-- ###   Use the given CSS or create your own :)   ### -->
    <!-- ################################################### -->

    <div class="max-w-[1440px] flex flex-wrap justify-center">
      <!-- Add Card component here!  -->
    </div>

    <!-- ############# PART 3: VUE DIRECTIVES!! ############### -->
    <!-- ###          Edit your Card component to           ###-->
    <!-- ###      create a list of cards using 'items'.     ### -->
    <!-- ###     Copy from items.txt to get your items :)   ### -->
    <!-- ###################################################### -->
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  data() {
    return {
      item: {
        id: '1',
        title1: 'Connect a Youth #HOGC21',
        title2: 'Connect a youth',
        description: 'Bringing a youth? Let us know! We’re here to help!',
        image: '',
      },
    }
  },
}
</script>
