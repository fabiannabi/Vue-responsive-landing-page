<template>
  <div class="heroes-body">
    <div class="heroes-title">
      <p>Become A Hero</p>
    </div>
    <div class="heroes-title--secnd">
      <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Eveniet, facere. Reiciendis alias iusto impedit non quasi</p>
    </div>
    <div v-for="hero in heroes" :key="hero.id">
      <div class="thumbnails">
        <figure class="thumbnail-hero">
          <img :src="hero.img" alt="hero" />
        </figure>
        <p class="description">{{hero.description}}</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "app",
  data() {
    return {
      heroes: [
        {
          img: "./src/assets/Tracer-profile.png",
          description:
            "Toting twin pulse pistols, energy-based time bombs, and rapid-fire banter, Tracer is able to 'blink' through space and rewind her personal timeline as she battles to right wrongs the world over."
        },
        {
          img: "./src/assets/Mercy-profile.png",
          description:
            "Mercy’s Valkyrie Suit helps keep her close to teammates like a guardian angel; healing, resurrecting or strengthening them with the beams emanating from her Caduceus Staff."
        },
        {
          img: "./src/assets/D.va-profile.png",
          description:
            "D.Va’s mech is nimble and powerful—its twin Fusion Cannons blast away with autofire at short range, and she can use its Boosters to barrel over enemies and obstacles, or deflect attacks with her projectile-dismantling Defense Matrix."
        },
        {
          img: "./src/assets/doomfist-profile.png",
          description:
            "Doomfist’s cybernetics make him a highly-mobile, powerful frontline fighter. In addition to dealing ranged damage with his Hand Cannon, Doomfist can slam the ground, knock enemies into the air and off balance, or charge into the fray with his Rocket Punch."
        }
      ]
    };
  }
};
</script>

<style lang="scss">
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
.thumbnails {
  align-items: center;
  justify-content: center;
  margin: auto;
  min-width: 500px;
  max-width: 750px;
  background-color: aqua;
  margin-bottom: 3rem;
  border-radius: 5px;
  padding: 2rem;
}
.thumbnail-hero {
  clip-path: circle(41.8% at 50% 50%);
  display: flex;
  justify-content: center;
}
.thumbnail-hero img {
  clip-path: circle(41.8% at 50% 50%);
  width: 20rem;
}
.description {
  font-size: 24px;
  text-align: justify;
  padding: 8px;
  font-family: "Open Sans", sans-serif;
  hyphens: auto;
}
.heroes-body {
  background-color: hsl(52, 55, 55);
  padding: 3rem 3rem;
}
.heroes-title {
  font-size: 60px;
  text-align: center;
  margin: 3rem;
  margin-bottom: 0;
  border-bottom: 0.5px solid black;
}
.heroes-title--secnd {
  font-size: 36px;
  text-align: center;
  margin: 7rem 1rem;
}
</style>
