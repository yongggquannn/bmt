<template>
  <div>
    <h1 class="text-3xl m-10 mb-4 font-bold">Happenings</h1>
    <p class="ml-10 mb-7">
      Stay in the know on the latest happenings & buzz in church!
    </p>

    <!-- ############# PART 2: PROPS & DATA!! ############## -->
    <!-- ###   Create your card using the 'item' below   ### -->
    <!-- ###   Use the given CSS or create your own :)   ### -->
    <!-- ################################################### -->
    <div class="max-w-[1440px] flex flex-wrap justify-center">
      <Card :item="item" />

      <!-- ############# PART 3: VUE DIRECTIVES!! ############## -->
      <!-- ###          Edit your Card component to          ### -->
      <!-- ###      create a list of cards using 'items'     ### -->
      <!-- ##################################################### -->

      <!-- <Card v-for="item in items" :key="item.id" :item="item" class="mb-5" /> -->
    </div>
  </div>
</template>

<script>
import Card from '~/components/Card.vue'
export default {
  name: 'IndexPage',
  component: { Card },
  data() {
    return {
      item: {
        id: '1',
        title1: 'CONNECT A YOUTH #HOGC21',
        title2: 'Connect a youth',
        description: 'Bringing a youth? Let us know! We’re here to help!',
        image: '',
      },
      items: [
        {
          id: '1',
          title1: 'CONNECT A YOUTH #HOGC21',
          title2: 'Connect a youth',
          description: 'Bringing a youth? Let us know! We’re here to help!',
          image: '',
        },
        {
          id: '2',
          title1: 'GET INVOLVED #HOGC21',
          title2: 'Get involved!',
          description: 'We need youth & we need YOU! Let’s reach down!',
          image: '',
        },
        {
          id: '3',
          title1: '',
          title2: 'HOGC21 Ideas',
          description: 'Want to do something but not sure how? Fret not!',
          image: '~/assets/images/hogc21.png',
        },
        {
          id: '4',
          title1: '',
          title2: 'Youth Events',
          description: 'Calling all young at heart',
          image: '~/assets/images/youth-events.png',
        },
        {
          id: '5',
          title1: '',
          title2: 'HeartKidz',
          description: 'Every Sat 5-7pm & Sun 1.30-3.30pm',
          image: '~/assets/images/heartkidz.png',
        },
        {
          id: '6',
          title1: '',
          title2: 'Service Replay',
          description: 'No FOMO! Sat 1.30pm & Sun 5pm',
          image: '~/assets/images/service-replay.png',
        },
      ],
    }
  },
}
</script>
