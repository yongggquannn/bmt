<template>
  <div>
    <div class="card">
      <!-- ####################################################################### -->
      <!-- ###           PART 2 HINT: Fill in the empty "top-title",           ### -->
      <!-- ###       "bottom-title" and "desc" with the prop attributes        ### -->
      <!-- ####################################################################### -->
      <div class="top-section">
        <h2 class="top-title"></h2>
      </div>

      <!-- #############    PART 3 HINT: Uncomment the div below    ############# -->
      <!-- <div class="image-container">
        <img class="image" :src="require(`~/assets/images/${item.image}.png`)" />
      </div> -->
      <!-- ###################################################################### -->

      <div class="bottom-section">
        <h3 class="bottom-title"></h3>
        <p class="desc"></p>
        <button class="button">Find out more</button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CardComponent',
  // PART 2 Hint: Add props here!
}
</script>

<style scoped>
.card {
  width: 300px;
  margin-right: 24px; /* 1.5rem */
  box-shadow: 0 20px 25px -5px rgb(0 0 0 / 0.1),
    0 8px 10px -6px rgb(0 0 0 / 0.1);
  border-radius: 12px; /* 0.75rem */
  overflow: hidden;
}

.top-section {
  display: flex;
  height: 180px;
  justify-content: center;
  align-items: center;
  background-color: #d3d8de;
  text-align: center;
}

.top-title {
  font-size: 24px; /* 1.5rem */
  line-height: 32px; /* 2rem */
  padding-left: 20px; /* 1.25rem */
  padding-right: 20px; /* 1.25rem */
  font-weight: 700;
}

.image-container {
  height: 180px;
}

.image {
  height: 180px;
  width: 100%;
}

.bottom-section {
  padding: 20px; /* 1.25rem */
}

.bottom-title {
  margin-bottom: 20px; /* 1.25rem */
  font-weight: 700;
}

.desc {
  margin-bottom: 20px; /* 1.25rem */
}

.button {
  background-color: #6245f4;
  color: white;
  padding: 12px; /* 0.75rem */
  border-radius: 12px; /* 0.75rem */
}
</style>
