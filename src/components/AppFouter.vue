<script>
export default {
  data() {
    return {
      buy: [
        {
          text: "DIGITAL COMICS",
          image: "buy-comics-digital-comics.png",
        },
        {
          text: "DC MERCHANDISE",
          image: "buy-comics-merchandise.png",
        },
        {
          text: "SUBCRIPTION",
          image: "buy-comics-subscriptions.png",
        },
        {
          text: "COMICS SHOP LOCATOR",
          image: "buy-comics-shop-locator.png",
        },
        {
          text: "DC POWER VISA",
          image: "buy-dc-power-visa.svg",
        },
      ],
      navList: [
        {
          title: "DC COMICS",
          listLink: [
            "Characters",
            "Comics",
            "Movies",
            "TV",
            "Games",
            "Videos",
            "News",
          ],
        },
        {
          title: "SHOP",
          listLink: ["Shop DC", "Shop DC Collectibles"],
        },
        {
          title: "DC",
          listLink: [
            "Terms Of Use",
            "Privacy policy (New)",
            "Ad Choises",
            "Advertising",
            "Jobs",
            "Subscriptions",
            "Talent Workshops",
            "CPSC Certificates",
            "Ratings",
            "Shop Help",
            "Contact Us",
          ],
        },
        {
          title: "SITES",
          listLink: [
            "DC",
            "MAD magazine",
            "DC Kids",
            "DC Universe",
            "DC Pover Visa",
          ],
        },
      ],
      social: [
        "footer-facebook.png",
        "footer-twitter.png",
        "footer-youtube.png",
        "footer-pinterest.png",
        "footer-periscope.png",
      ],
    };
  },

  methods: {
    imageGenerate(imageName) {
      const imageUrl = new URL("../assets/img/" + imageName, import.meta.url);

      return imageUrl.href;
    },
  },
};
</script>

<template>
  <footer>
    <section class="buy-container">
      <div class="container">
        <ul>
          <li v-for="buyItem in buy">
            <img :src="imageGenerate(buyItem.image)" alt="{{ buyItem.text }}" />
            <p>{{ buyItem.text }}</p>
          </li>

          <!-- Base di partenza
          <li>
            <img src="../assets/img/buy-dc-power-visa.svg" alt="icona" />
            <p>DIGITAL COMICS</p>
          </li> -->
        </ul>
      </div>
    </section>
    <section class="nav_container">
      <div class="container">
        <nav>
          <div v-for="navListItem in navList">
            <h1>{{ navListItem.title }}</h1>
            <ul>
              <li v-for="link in navListItem.listLink">
                <p>
                  <a href="#">{{ link }}</a>
                </p>
              </li>
            </ul>
          </div>
          <!-- BASE DI PARTENZA
          <div>
            <h1>Dc comics</h1>
            <ul>
              <li>
                <p><a href="#">Characters</a></p>
              </li>
              <li>
                <p><a href="#">Characters</a></p>
              </li>
              <li>
                <p><a href="#">Characters</a></p>
              </li>
              <li>
                <p><a href="#">Characters</a></p>
              </li>
              <li>
                <p><a href="#">Characters</a></p>
              </li>
              <li>
                <p><a href="#">Characters</a></p>
              </li>
              <li>
                <p><a href="#">Characters</a></p>
              </li>
            </ul>
          </div>
          <div>
            <h1>Dc comics</h1>
            <ul>
              <li>
                <p><a href="#">Characters</a></p>
              </li>
              <li>
                <p><a href="#">Shop DC collectible</a></p>
              </li>
            </ul>
          </div>
          <div>
            <h1>Dc comics</h1>
            <ul>
              <li>
                <p><a href="#">Characters</a></p>
              </li>
              <li>
                <p><a href="#">Characters</a></p>
              </li>
              <li>
                <p><a href="#">Characters</a></p>
              </li>
              <li>
                <p><a href="#">Characters</a></p>
              </li>
              <li>
                <p><a href="#">Characters</a></p>
              </li>
              <li>
                <p><a href="#">Characters</a></p>
              </li>
              <li>
                <p><a href="#">Characters</a></p>
              </li>
              <li>
                <p><a href="#">Characters</a></p>
              </li>
              <li>
                <p><a href="#">Characters</a></p>
              </li>
              <li>
                <p><a href="#">Characters</a></p>
              </li>
              <li>
                <p><a href="#">Characters</a></p>
              </li>
              <li>
                <p><a href="#">Characters</a></p>
              </li>
              <li>
                <p><a href="#">Characters</a></p>
              </li>
            </ul>
          </div>
          <div>
            <h1>Dc comics</h1>
            <ul>
              <li>
                <p><a href="#">Characters</a></p>
              </li>
              <li>
                <p><a href="#">Characters</a></p>
              </li>
              <li>
                <p><a href="#">Characters</a></p>
              </li>
              <li>
                <p><a href="#">Characters</a></p>
              </li>
              <li>
                <p><a href="#">Characters</a></p>
              </li>
            </ul>
          </div> -->
        </nav>
      </div>
    </section>
    <section class="social-container">
      <div class="container social">
        <h3><a href="#">SIGN-UP NOW!</a></h3>
        <div class="social-icon">
          <h2>FOLLOW US</h2>
          <a v-for="iconLink in social" href="#">
            <img :src="imageGenerate(iconLink)" alt="{{iconLink}}" />
          </a>
          <!-- BASE DI PARTENZA
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
          </a> -->
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
    height: 50px;
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
