<template>
  <div class="teams-body">
    <div class="teams-title">
      <p>Pro League Teams</p>
    </div>
    <div class="teams-title--secnd">
      <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Eveniet, facere. Reiciendis alias iusto impedit non quasi</p>
    </div>
    <carousel
      class="carousel-teams"
      :autoplay="true"
      :nav="false"
      :loop="true"
      :dots="false"
      :items="1"
    >
      <img src="../assets/soul.png" />
      <img src="../assets/huston.png" />
      <img src="../assets/london.png" />
      <img src="../assets/ny.png" />
      <img src="../assets/shock.png" />
      <img src="../assets/boston.png" />
      <img src="../assets/dragons.png" />
      <img src="../assets/fuel.png" />
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
<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.teams-body {
  padding: 3rem 3rem;
}
.teams-title {
  font-size: 60px;
  text-align: center;
  margin: 3rem;
  margin-bottom: 0;
  border-bottom: 0.5px solid black;
}
.teams-title--secnd {
  font-size: 36px;
  text-align: center;
  margin: 7rem 1rem;
  color: hsl(212, 18%, 35%);
}
.carousel-teams {
  box-shadow: 0 5px 15px hsl(212, 18%, 35%);
}
@media (min-width: 1000px) {
  .teams-title--secnd {
    font-size: 40px;
    text-align: center;
    margin: 7rem 1rem;
    color: hsl(212, 18%, 35%);
  }
}
</style>
