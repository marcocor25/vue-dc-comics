<template>
  <div class="container-fluid">
    <div class="container">
      <div class="list-col">
        <div class="list-wrapper">
          <!-- LISTA 1 -->
          <ul>
            <h2>{{ title1 }}</h2>
            <li v-for="(element, index) in list1" :key="index">
              {{ element.text }}
            </li>
          </ul>
          <!-- LISTA 4 -->
          <ul>
            <h2>{{ title4 }}</h2>
            <li v-for="(element, index) in list4" :key="index">
              {{ element.text }}
            </li>
          </ul>
        </div>
        <!-- LISTA 2 -->
        <ul>
          <h2>{{ title2 }}</h2>
          <li v-for="(element, index) in list2" :key="index">
            {{ element.text }}
          </li>
        </ul>
        <!-- LISTA 3 -->
        <ul>
          <h2>{{ title3 }}</h2>
          <li v-for="(element, index) in list3" :key="index">
            {{ element.text }}
          </li>
        </ul>
      </div>
      <!-- BACKGROUND LOGO DC -->
      <div class="logo-col"></div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MyFooter",
  data() {
    return {
      title1: "dc comics",
      title2: "dc",
      title3: "sites",
      title4: "shop",
      list1: [
        {
          text: "Characters",
        },
        {
          text: "Comics",
        },
        {
          text: "Movie",
        },
        {
          text: "TV",
        },
        {
          text: "Games",
        },
        {
          text: "Videos",
        },
        {
          text: "News",
        },
      ],
      list2: [
        {
          text: "Terms Of Use",
        },
        {
          text: "Privacy Policy (New)",
        },
        {
          text: "Ad Choices",
        },
        {
          text: "Advertising",
        },
        {
          text: "Jobs",
        },
        {
          text: "Subscription",
        },
        {
          text: "Talent Workshops",
        },
        {
          text: "CPSC Certificates",
        },
        {
          text: "Ratings",
        },
        {
          text: "Shop Help",
        },
        {
          text: "Contact Us",
        },
      ],
      list3: [
        {
          text: "DC",
        },
        {
          text: "MAD Magazine",
        },
        {
          text: "DC Kids",
        },
        {
          text: "DC Universe",
        },
        {
          text: "DC Power Visa",
        },
      ],
      list4: [
        {
          text: "Shop DC",
        },
        {
          text: "Shop DC collectibles",
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container-fluid {
  background-image: url("../assets/img/footer-bg.jpg");
  background-size: cover;
  background-position: center;

  .container {
    width: 1000px;
    min-height: 300px;
    margin: 0 auto;
    display: flex;
    color: #fffffd;

    .list-col {
      width: 60%;
      padding: 20px 0;
      display: flex;
      gap: 30px;

      h2 {
        padding: 10px 0;
        text-transform: uppercase;
      }

      li {
        cursor: pointer;
        color: #788d77;

        &:hover {
          color: #fffffd;
          text-decoration: underline;
        }
      }
    }

    .logo-col {
      width: 40%;
      background-image: url("../assets/img/dc-logo-bg.png");
      background-size: cover;
      background-position: center;
    }
  }
}
</style>