<template>
  <div>
    <div class="header">
      <div class="header-logo">
        <img src="../assets/pngocean.com.png" alt />
      </div>
    </div>
    <div class="btn">
      <button>Play it Now</button>
    </div>
  </div>
</template>

<script>
export default {
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

.header {
  width: 100vw;
  height: 500px;
  background-size: cover;
}
.header-logo {
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: hsl(210, 38%, 93%);
}
.header-logo img {
  display: flex;
  width: 800px;
  margin: 4rem;
}

.btn {
  display: flex;
  align-content: center;
  justify-content: center;
  margin: 2rem;
}

button {
  background-image: linear-gradient(
    to bottom,
    hsl(50, 100%, 50%),
    hsl(32, 100%, 50%)
  );
  width: 100%;
  margin: 16px;
  padding: 12px 29px;
  border-radius: 15px;
  font-family: "Open Sans", sans-serif;
  height: 6rem;
  font-size: 58px;
  color: hsl(32, 100%, 20%);
  box-shadow: 0 5px 10px hsl(212, 18%, 35%), 0 2px 5px hsl(212, 18%, 35%);
}

@media only screen and (min-width: 1000px) {
  button {
    background-color: red;
    width: 30%;
    margin: 15px;
    padding: 12px 29px;
    border-radius: 15px;
    font-family: "Open Sans", sans-serif;
    height: 4rem;
    font-size: 29px;
  }
}
</style>
