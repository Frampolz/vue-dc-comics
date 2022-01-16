<template>
  <div class="container d-flex">
    <div class="logo">
      <img src="../assets/img/dc-logo.png" alt="" />
    </div>
    <div class="menu">
      <ul>
        <li
          v-for="(link, index) in links"
          :key="index"
        >
          <a :href="link.url" @click="newFuction(index)"
          :class="(link.linkIndex == true) ? 'active' : ''">{{ link.text }}</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      links: [
        {
          text: "character",
          linkIndex: false,
          url: "#",
        },
        {
          text: "comics",
          linkIndex: true,
          url: "#",
        },
        {
          text: "movie",
          linkIndex: false,
          url: "#",
        },
        {
          text: "tv",
          linkIndex: false,
          url: "#",
        },
        {
          text: "games",
          linkIndex: false,
          url: "#",
        },
        {
          text: "collectibles",
          linkIndex: false,
          url: "#",
        },
        {
          text: "videos",
          linkIndex: false,
          url: "#",
        },
        {
          text: "fans",
          linkIndex: false,
          url: "#",
        },
        {
          text: "news",
          linkIndex: false,
          url: "#",
        },
        {
          text: "shop",
          linkIndex: false,
          url: "#",
        },
      ],
    };
  },
  methods: {
    newFuction: function (index) {
        this.links.forEach((element, elementindex) => {
            if (elementindex == index) {
                element.linkIndex = true
            } else {
                element.linkIndex = false
                
            }
        });

    },
  },
};
</script>

<style lang="scss" scoped>
@import "../assets/scss/partials/_variables.scss";

.container {
  justify-content: space-between;
  text-transform: uppercase;
}
img {
  padding: 1em;
}
ul {
  li {
    display: inline-block;
    padding: 1em;

    a {
      text-decoration: none;
      padding: 3.8em 0;
      color: $headerLiColor;
      font-weight: bold;
      font-size: 0.8em;
      transition: all .3s;
      &:hover,
      &:active,
      &.active {
        color: $blueColor;
        border-bottom: 5px solid $blueColor;
      }
    }
  }
}
</style>
