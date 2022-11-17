<template>
  <div>
    <h1 class="text-3xl mb-4">Question Extra</h1>

    <!-- ############# PART 2: PROPS & DATA!! ############## -->
    <!-- ###   Create your card using the 'item' below   ### -->
    <!-- ###   Use the given CSS or create your own :)   ### -->
    <!-- ################################################### -->
    <div class="cards-section">
      <Card v-for="item in items" :key="item" :item="item" />
    </div>
  </div>
</template>

<script>
import Card from '~/components/Card'
export default {
  name: 'IndexPage',
  component: { Card },
  data() {
    return {
      item: [
        {
          title1: 'CONNECT A YOUTH #HOGC21',
          title2: 'Connect a youth',
          description: 'Bringing a youth? Let us know! We’re here to help!',
          image: '',
        },
      ],
      items: [
        {
          title1: 'CONNECT A YOUTH #HOGC21',
          title2: 'Connect a youth',
          description: 'Bringing a youth? Let us know! We’re here to help!',
          image: '',
        },
        {
          title1: 'GET INVOLVED #HOGC21',
          title2: 'Get involved!',
          description: 'We need youth & we need YOU! Let’s reach down!',
          image: '',
        },
        {
          title1: '',
          title2: 'HOGC21 Ideas',
          description: 'Want to do something but not sure how? Fret not!',
          image: '~/assets/images/hogc21.png',
        },
        {
          title1: '',
          title2: 'Youth Events',
          description: 'Calling all young at heart',
          image: '~/assets/images/youth-events.png',
        },
        {
          title1: '',
          title2: 'HeartKidz',
          description: 'Every Sat 5-7pm & Sun 1.30-3.30pm',
          image: '~/assets/images/heartkidz.png',
        },
        {
          title1: '',
          title2: 'Service Replay',
          description: 'No FOMO! Sat 1.30pm & Sun 5pm',
          image: '~/assets/images/service-replay.png',
        },
        {
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
.card-container {
  font-family: 'Roboto', sans-serif;
  filter: drop-shadow(0px 1px 25px rgba(0, 0, 0, 0.25));
  width: 300px;
  border-radius: 12px;
  border: 0.5px solid rgba(0, 0, 0, 0.25);
  margin-right: 24px;
  margin-bottom: 48.5px;
}

.card-image {
  height: 200px;
  width: 100%;
  /* border-top-left-radius: ...  */
  /* border-top-right-radius: ...  */
  /* display: ... */
  /* justify-content: ... 
        /* align-items: ... */
  color: #fff;
  font-size: 5rem;
}

.card-content {
  padding: 20px 24px;
}

.cards-section {
  display: flex;
  /* flex-direction: ... */
  justify-content: center;
  flex-wrap: wrap;
  max-width: 1440px;
  /* padding: 0 156px; */
  /* margin: auto; */
}

.card-title {
  font-weight: bold;
  font-size: 18px;
  margin-bottom: 8px;
}

.cards {
  display: flex;
}
</style>
