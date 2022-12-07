<template>
  <div>
    <div class="top-banner">
      <!-- ############# PART 1: PROJ STRUCTURE!! ############## -->
      <!-- ###      Add in HOGC Logo into assets folder,     ### -->
      <!-- ###      and add the file path in the img tag     ### -->
      <!-- ##################################################### -->

      <!-- <img class="logo" src="??" /> -->

      <h3 class="banner-title">HOGC One</h3>
    </div>
    <h1 class="title">Happenings</h1>
    <p class="desc">
      Stay in the know on the latest happenings & buzz in church!
    </p>

    <!-- ############# PART 2: PROPS & DATA!! ############## -->
    <!-- ###   Create your card using the 'item' below   ### -->
    <!-- ###   Use the given CSS or create your own :)   ### -->
    <!-- ################################################### -->

    <div class="cards-container">
      <!-- Add Card component here!  -->
    </div>

    <!-- ############# PART 3: VUE DIRECTIVES!! ############## -->
    <!-- ###          Edit your Card component to          ### -->
    <!-- ###      create a list of cards using 'items'     ### -->
    <!-- ##################################################### -->
  </div>
</template>

<script>
// PART 2 Hint: Add import here!
export default {
  // PART 2 Hint: Add component here!
  name: 'IndexPage',
}
</script>

<style scoped>
.top-banner {
  display: flex;
  background-image: linear-gradient(to right, var(--tw-gradient-stops));
  --tw-gradient-from: #ffe543;
  --tw-gradient-to: #ffcd19;
  --tw-gradient-stops: var(--tw-gradient-from), var(--tw-gradient-to);
  padding: 28px; /* 1.75rem */
  padding-left: 40px; /* 2.5rem */
  margin-bottom: 28px; /* 1.75rem */
}

.logo {
  margin-right: 20px; /* 1.25rem */
}

.banner-title {
  font-size: 24px; /* 1.5rem */
  line-height: 32px; /* 2rem */
  font-weight: 700;
}

.title {
  font-size: 30px; /* 1.875rem */
  line-height: 36px; /* 2.25rem */
  margin: 40px; /* 2.5rem */
  margin-bottom: 20px; /* 1.25rem */
  font-weight: 700;
}

.desc {
  margin-left: 40px; /* 2.5rem */
  margin-right: 40px; /* 2.5rem */
  margin-bottom: 24px; /* 1.5rem */
}

.cards-container {
  max-width: 1440px;
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
</style>
