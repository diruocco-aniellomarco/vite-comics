<script>
export default {
  data() {
    return {
      title: "Ciao",
    };
  },
};
</script>

<template>
  <footer>
    <section class="buy-container">
      <div class="container">
        <ul>
          <li>
            <img src="../assets/img/buy-dc-power-visa.svg" alt="icona" />
            <p>DIGITAL COMICS</p>
          </li>

          <li>
            <img src="../assets/img/buy-dc-power-visa.svg" alt="icona" />
            <p>DIGITAL COMICS</p>
          </li>

          <li>
            <img src="../assets/img/buy-dc-power-visa.svg" alt="icona" />
            <p>DIGITAL COMICS</p>
          </li>

          <li>
            <img src="../assets/img/buy-dc-power-visa.svg" alt="icona" />
            <p>DIGITAL COMICS</p>
          </li>

          <li>
            <img src="../assets/img/buy-dc-power-visa.svg" alt="icona" />
            <p>DIGITAL COMICS</p>
          </li>
        </ul>
      </div>
    </section>
    <section class="nav_container">
      <div class="container">
        <nav>
          <ul>
            <li class="title-list"><h1>Dc comics</h1></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
          </ul>

          <ul>
            <li class="title-list"><h1>Dc comics</h1></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
          </ul>

          <ul>
            <li class="title-list"><h1>Dc comics</h1></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
          </ul>

          <ul>
            <li class="title-list"><h1>Dc comics</h1></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
          </ul>
        </nav>
      </div>
    </section>
    <section></section>
  </footer>
</template>

<style lang="scss" scoped>
.buy-container {
  background-color: #0282f9;
  color: white;
  height: 150px;
  line-height: 150px;

  img {
    width: 50px;
  }

  li {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 10px;
  }

  ul {
    width: 100%;
    display: flex;
    justify-content: space-around;
  }
}

.nav_container {
  background-image: url(../assets/img/footer-bg.jpg);
  height: 400px;

  nav {
    padding-top: 20px;
    color: white;
    height: 100%;
    display: flex;
    flex-direction: column;
    flex-wrap: wrap;
    height: 400px;
    gap: 25px;

    li {
      display: block;
      margin: 0;
      line-height: 25px;

      .title-list {
        margin-top: 10px;
        margin-bottom: 10px;
      }

      p {
        font-size: small;
        color: gray;
      }
    }
  }
}
</style>
