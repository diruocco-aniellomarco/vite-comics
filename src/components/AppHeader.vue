<script>
export default {
  data() {
    return {
      pages: [
        "CHARACTERS",
        "COMICS",
        "MOVIES",
        "TV",
        "GAMES",
        "COLLECTIBLES",
        "VIDEOS",
        "FANS",
        "NEWS",
        "SHOP",
      ],
    };
  },
};
</script>

<template>
  <header>
    <div class="container">
      <div>
        <img src="../assets/img/dc-logo.png" alt="logo" />
      </div>
      <div>
        <ul>
          <li v-for="page in pages">
            <p>
              <a href="#">{{ page }}</a>
            </p>
          </li>
          <!-- <li><a href="#">Ciao</a></li>
          <li><a href="#">Ciao</a></li>
          <li><a href="#">Ciao</a></li>
          <li><a href="#">Ciao</a></li>
          <li><a href="#">Ciao</a></li>
          <li><a href="#">Ciao</a></li>
          <li><a href="#">Ciao</a></li>
          <li><a href="#">Ciao</a></li>
          <li><a href="#">miao</a></li> -->
        </ul>
      </div>
    </div>
  </header>
</template>

<style lang="scss" scoped>
img {
  width: 70px;
}

li {
  height: 100px;
  line-height: 100px;
}

header::after {
  content: "";
  display: block;
  height: 300px;
  background-image: url("../assets/img/jumbotron.jpg");
}
</style>
