<template>
  <div class="heroes-body">
    <div class="heroes-title">
      <p>Become A Hero</p>
    </div>
    <div class="heroes-title--secnd">
      <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Eveniet, facere. Reiciendis alias iusto impedit non quasi</p>
    </div>
    <div class="cards">
      <div v-for="hero in heroes" :key="hero.id">
        <div class="thumbnails">
          <p class="name">{{hero.name}}</p>
          <div class="cards-inner">
            <figure class="thumbnail-hero">
              <img :src="hero.img" alt="hero" />
            </figure>
            <p class="description">{{hero.description}}</p>
          </div>
        </div>
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
          name: "Tracer",
          img: "./src/assets/Tracer-profile.png",
          description:
            "Toting twin pulse pistols, energy-based time bombs, and rapid-fire banter, Tracer is able to 'blink' through space and rewind her personal timeline as she battles to right wrongs the world over."
        },
        {
          name: "Mercy",
          img: "./src/assets/Mercy-profile.png",
          description:
            "Mercy’s Valkyrie Suit helps keep her close to teammates like a guardian angel; healing, resurrecting or strengthening them with the beams emanating from her Caduceus Staff."
        },
        {
          name: "D.va",
          img: "./src/assets/D.va-profile.png",
          description:
            "D.Va’s mech is nimble and powerful—its twin Fusion Cannons blast away with autofire at short range, and she can use its Boosters to barrel over enemies and obstacles, or deflect attacks with her projectile-dismantling Defense Matrix."
        },
        {
          name: "Doomfist",
          img: "./src/assets/doomfist-profile.png",
          description:
            "Doomfist’s cybernetics make him a highly-mobile, powerful frontline fighter. In addition to dealing ranged damage with his Hand Cannon, Doomfist can slam the ground, knock enemies into the air and off balance."
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
  background-color: hsl(210, 90%, 97%);
  margin-bottom: 3rem;
  border-radius: 5px;
  padding: 2rem;
  box-shadow: 0 5px 10px hsl(212, 18%, 35%);
}

.thumbnail-hero {
  clip-path: circle(41.8% at 50% 50%);
  display: flex;
  justify-content: space-around;
  align-content: center;
}
.thumbnail-hero img {
  clip-path: circle(41.8% at 50% 50%);
  width: 20rem;
}
.name {
  font-family: "Open Sans", sans-serif;
  font-size: 40px;
  text-align: center;
  font-weight: bold;
  padding: 1.5rem;
  border-bottom: 0.5px dotted black;
}
.description {
  font-size: 24px;
  text-align: justify;
  padding: 1.5rem;
  font-family: "Open Sans", sans-serif;
  hyphens: auto;
  background-color: hsl(210, 90%, 95%);
  color: hsl(212, 20%, 35%);
  line-height: 1.3;
}
.heroes-body {
  background-color: hsl(210, 32%, 93%);
  padding: 2rem 2rem;
}
.heroes-title {
  font-size: 60px;
  text-align: center;
  margin: 3rem;
  margin-bottom: 0;
  border-bottom: 0.5px solid black;
  color: hsl(212, 56%, 16%);
}
.heroes-title--secnd {
  font-size: 36px;
  text-align: center;
  margin: 7rem 1rem;
  color: hsl(212, 18%, 35%);
}

@media (min-width: 1000px) {
  .cards {
    display: flex;
    justify-content: center;
    align-content: center;
    flex-wrap: wrap;
  }
  .cards-inner {
    display: flex;
    margin: 1rem 1rem;
  }
  .thumbnails {
    display: flex;
    flex-direction: column;
    margin-left: 6rem;
    margin-right: 3rem;
    align-content: center;
    height: 300px;
    width: 800px;
    background-color: hsl(210, 90%, 97%);
    margin-bottom: 3rem;
    border-radius: 5px;
    box-shadow: 0 5px 10px hsl(212, 18%, 35%);
  }
  .name {
    font-family: "Open Sans", sans-serif;
    font-size: 20px;
    text-align: center;
    font-weight: bold;
    padding: 1rem;
    border-bottom: 0.5px dotted black;
  }
  .description {
    font-size: 16px;
    text-align: justify;
    padding: 1.5rem;
    font-family: "Open Sans", sans-serif;
    hyphens: auto;
    background-color: hsl(210, 90%, 95%);
    color: hsl(212, 20%, 35%);
    line-height: 1.3;
  }
  .heroes-title--secnd {
    font-size: 40px;
    text-align: center;
    margin: 7rem 1rem;
    color: hsl(212, 18%, 35%);
  }
  .thumbnail-hero {
    clip-path: circle(41.8% at 50% 50%);
    display: flex;
    justify-content: center;
  }
  .thumbnail-hero img {
    clip-path: circle(41.8% at 50% 50%);
    width: 8rem;
    margin-right: 1rem;
  }
  .heroes-title {
    font-size: 60px;
    text-align: center;
    margin: 3rem;
    margin-bottom: 0;
    border-bottom: 0.5px solid black;
    color: hsl(212, 56%, 16%);
  }
}
</style>
