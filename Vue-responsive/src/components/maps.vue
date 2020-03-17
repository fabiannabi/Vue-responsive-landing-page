<template>
  <div class="maps-body">
    <div class="maps-title">
      <p>Travel The World</p>
    </div>
    <div class="maps-title--secnd">
      <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Eveniet, facere. Reiciendis alias iusto impedit non quasi</p>
    </div>
    <carousel
      class="carousel-maps"
      :autoplay="true"
      :nav="false"
      :loop="true"
      :dots="false"
      :items="1"
    >
      <img src="../assets/ayutthaya.jpg" />
      <img src="../assets/black-forest.jpg" />
      <img src="../assets/blizzard-world.jpg" />
      <img src="../assets/busan.jpg" />
      <img src="../assets/dorado.jpg" />
      <img src="../assets/eichenwalde.jpg" />
      <img src="../assets/hanamura.jpg" />
      <img src="../assets/junkertown.jpg" />
    </carousel>
  </div>
</template>

<script>
import carousel from "vue-owl-carousel";
export default {
  components: { carousel },
  name: "app",
  data() {
    return {};
  }
};
</script>
<style lang="scss" 
>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.maps-body {
  padding: 3rem 3rem;
}
.maps-title {
  font-size: 60px;
  text-align: center;
  margin: 3rem;
  margin-bottom: 0;
  border-bottom: 0.5px solid black;
}
.maps-title--secnd {
  font-size: 36px;
  text-align: center;
  margin: 7rem 1rem;
}
.carousel-maps {
  box-shadow: 0 5px 15px hsl(212, 18%, 35%);
}

@media (min-width: 1000px) {
  .maps-title--secnd {
    font-size: 40px;
    text-align: center;
    margin: 7rem 1rem;
    color: hsl(212, 18%, 35%);
  }
}
</style>
