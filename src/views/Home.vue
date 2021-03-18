<template>
  <div class="home">
    <carousel :autoplay="false" :items="1" :nav="false">
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
  padding: 0 var(--padding);
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

.owl-theme .owl-dots .owl-dot.active span,
.owl-theme .owl-dots .owl-dot:hover span {
  background-color: var(--secondary) !important;
}

.bar {
  display: flex;
  flex-direction: row;
  justify-content: space-around;
  width: 100%;
  padding: 15px 0;
  margin-top: -23px;
  margin: -23px 0 var(--defaultSpace);
  background-color: var(--secondary);
}
</style>
