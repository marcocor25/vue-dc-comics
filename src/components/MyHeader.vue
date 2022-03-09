<template>
  <div class="container-fluid">
    <div class="container">
      <figure class="logo">
        <img src="../assets/img/dc-logo.png" />
      </figure>

      <div class="nav-link">
        <ul>
          <li v-for="(element, index) in link" :key="index">
            <a :href="element.href">{{ element.text }}</a>
          </li>
        </ul>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MyHeader",
  data() {
    return {
      link: [
        {
          text: "characters",
          href: "#",
        },
        {
          text: "comics",
          href: "#",
        },
        {
          text: "movies",
          href: "#",
        },
        {
          text: "tv",
          href: "#",
        },
        {
          text: "games",
          href: "#",
        },
        {
          text: "collectibles",
          href: "#",
        },
        {
          text: "videos",
          href: "#",
        },
        {
          text: "fans",
          href: "#",
        },
        {
          text: "news",
          href: "#",
        },
        {
          text: "shop",
          href: "#",
        },
      ],
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.container-fluid {
  background: white;

  .container {
    width: 1000px;
    min-height: 80px;
    margin: 0 auto;
    display: flex;
    justify-content: space-between;
    align-items: center;

    .logo {
      width: 60px;
      height: 60px;
    }

    .nav-link {
      ul {
        display: flex;
        gap: 20px;
      }

      li {
        line-height: 77px;
        border-bottom: 3px solid transparent;
        font-size: 11px;
        cursor: pointer;
        transition: 200ms linear;

        &:hover {
          border-bottom: 3px solid #0082f9;
        }
      }

      a {
        font-weight: 700;
        text-decoration: none;
        text-transform: uppercase;
        color: currentColor;
      }
    }
  }
}
</style>