<template>
  <div>
    <h1 class="text-3xl mb-4">Question Extra</h1>

    <!-- ############# PART 2: PROPS & DATA!! ############## -->
    <!-- ###   Create your card using the 'item' below   ### -->
    <!-- ###   Use the given CSS or create your own :)   ### -->
    <!-- ################################################### -->
    <div class="cards-section">
      <Card v-for="item in items" :key="item.id" :item="item" />
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
      item: [
        {
          id: '1',
          title1: 'CONNECT A YOUTH #HOGC21',
          title2: 'Connect a youth',
          description: 'Bringing a youth? Let us know! We’re here to help!',
          image: '',
        },
      ],
      items: [
        {
          id: '2',
          title1: 'CONNECT A YOUTH #HOGC21',
          title2: 'Connect a youth',
          description: 'Bringing a youth? Let us know! We’re here to help!',
          image: '',
        },
        {
          id: '3',
          title1: 'GET INVOLVED #HOGC21',
          title2: 'Get involved!',
          description: 'We need youth & we need YOU! Let’s reach down!',
          image: '',
        },
        {
          id: '4',
          title1: '',
          title2: 'HOGC21 Ideas',
          description: 'Want to do something but not sure how? Fret not!',
          image: '~/assets/images/hogc21.png',
        },
        {
          id: '5',
          title1: '',
          title2: 'Youth Events',
          description: 'Calling all young at heart',
          image: '~/assets/images/youth-events.png',
        },
        {
          id: '6',
          title1: '',
          title2: 'HeartKidz',
          description: 'Every Sat 5-7pm & Sun 1.30-3.30pm',
          image: '~/assets/images/heartkidz.png',
        },
        {
          id: '7',
          title1: '',
          title2: 'Service Replay',
          description: 'No FOMO! Sat 1.30pm & Sun 5pm',
          image: '~/assets/images/service-replay.png',
        },
        {
          id: '8',
          title1: 'CONNECT A YOUTH #HOGC21',
          title2: 'Connect a youth',
          description: 'Bringing a youth? Let us know! We’re here to help!',
          image: '',
        },
      ],
    }
  },
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Roboto&display=swap');

.cards-section {
  display: flex;
  /* flex-direction: ... */
  justify-content: center;
  flex-wrap: wrap;
  max-width: 1440px;
  /* padding: 0 156px; */
  /* margin: auto; */
  border: 2px;
  border-color: black;
}
</style>
