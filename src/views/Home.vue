<template>
  <div class="home">
    <carousel :autoplay="true" :items="1" :nav="false">
      <img src="https://placeimg.com/1366/768/any?1">
      <img src="https://placeimg.com/1366/768/any?2">
      <img src="https://placeimg.com/1366/768/any?3">
      <img src="https://placeimg.com/1366/768/any?4">
    </carousel>

    <div class="bar">
      <div class="bar-item-box-1">placeholder item</div>
      <div class="bar-item-box-2">placeholder item</div>
      <div class="bar-item-box-3">placeholder item</div>
      <div class="bar-item-box-4">placeholder item</div>
    </div>
  </div>
</template>

<script>
import carousel from 'vue-owl-carousel'

export default {
  name: 'Home',
  components: {
    carousel
  }
}
</script>

<style>
.home {
  padding: 0 15px;
}

@media (max-width: 700px) {
  .home {
    padding: 0 7.5px;
  }
}

.owl-theme .owl-nav.disabled + .owl-dots {
  margin-top: 0;
}

.owl-theme .owl-dots {
  position: relative;
  top: -30px;
}

.bar {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  width: 100%;
  padding: 15px 0;
  margin-top: -23px;
  background-color: var(--secondary);
}
</style>
