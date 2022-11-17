<template>
  <div>
    <!-- <h1 class="text-3xl mb-4">Question Extra</h1> -->
    <!-- Qn: Use v-for directive to render a list of items based on a given array. -->
    <!-- Display them in cards form. (Refer to the image in the assets folder) -->
    <!-- There are missing css styling too. -->
    <div class="card-container card-content">
      <div v-if="item.image === ''">
        <h3>{{ item.title1 }}</h3>
      </div>
      <div v-else class=""></div>
      <div>
        <h3 class="card-title">{{ item.title2 }}</h3>
        <p>{{ item.description }}</p>
        <button>Find out more</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CardDefault',
  methods: {
    header(color) {
      let stylename = 'background-color: '
      stylename += color
      return stylename
    },
  },
  props: {
    item: {
      type: Object,
      required: true,
    },
  },
  // data() {
  //   return {
  //     items: [
  //       {
  //         title: 'Trousers',
  //         id: 1,
  //         description: 'Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum',
  //         color: '#75C2EC',
  //       },
  //       {
  //         title: 'Shirt',
  //         id: 2,
  //         description: 'Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum',
  //         color: '#F6C42E',
  //       },
  //       {
  //         title: 'Coat',
  //         id: 3,
  //         description: 'Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum',
  //         color: '#007C00',
  //       },
  //       {
  //         title: 'Dress',
  //         id: 4,
  //         description: 'Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum',
  //         color: '#75C2EC',
  //       },
  //       {
  //         title: 'Blouse',
  //         id: 5,
  //         description: 'Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum',
  //         color: '#F6C42E',
  //       },
  //       {
  //         title: 'Sock',
  //         id: 6,
  //         description: 'Lorem Ipsum Lorem Ipsum Lorem Ipsum Lorem Ipsum',
  //         color: '#007C00',
  //       },
  //     ],
  //   }
  // },
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
