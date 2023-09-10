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
          <h1>Dc comics</h1>
          <ul>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
          </ul>
          <h1>Dc comics</h1>
          <ul>
            <li><p>Characters</p></li>
            <li><p>Shop DC collectible</p></li>
          </ul>
          <h1>Dc comics</h1>
          <ul>
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
          <h1>Dc comics</h1>
          <ul>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
            <li><p>Characters</p></li>
          </ul>
        </nav>
      </div>
    </section>
    <section class="social-container">
      <div class="container social">
        <h3><a href="#">SIGN-UP NOW!</a></h3>
        <div class="social-icon">
          <h2>FOLLOW US</h2>
          <a href="#">
            <img src="../assets/img/footer-facebook.png" alt="" /> </a
          ><a href="#">
            <img src="../assets/img/footer-twitter.png" alt="" /> </a
          ><a href="#">
            <img src="../assets/img/footer-youtube.png" alt="" /> </a
          ><a href="#">
            <img src="../assets/img/footer-pinterest.png" alt="" /> </a
          ><a href="#">
            <img src="../assets/img/footer-periscope.png" alt="" />
          </a>
        </div>
      </div>
    </section>
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

.social-container {
  background-color: #303030;
  padding: 20px 0;
  .social {
    display: flex;
    justify-content: space-between;

    h3 {
      color: white;
      padding: 20px;
      border: 2px solid #0282f9;
    }
    .social-icon {
      display: flex;
      align-items: center;
      justify-content: flex-end;
      gap: 20px;

      h2 {
        color: #0282f9;
      }
    }
  }
}
</style>
