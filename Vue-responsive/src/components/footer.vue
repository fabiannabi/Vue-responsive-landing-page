<template>
  <div class="footer">
    <ul>
      <li>
        <a href="https://playoverwatch.com/en-us/">
          <img src="https://picsum.photos/100/100" alt />
        </a>
      </li>
    </ul>
    <ul>
      <li>
        <a href="https://www.youtube.com/PlayOverwatch">
          <img src="https://picsum.photos/100/100" alt />
        </a>
      </li>
    </ul>
    <ul>
      <li>
        <a href="https://twitter.com/playoverwatch">
          <img src="https://picsum.photos/100/100" alt />
        </a>
      </li>
    </ul>
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
<style lang="scss" >
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

.footer {
  padding: 3rem;
  background-color: rgb(164, 197, 197);
  display: flex;
  align-items: center;
  justify-content: space-around;
  list-style: none;
}
.footer li {
  list-style: none;
  border-radius: 100%;
}
.footer li img {
  border-radius: 100%;
}
</style>
