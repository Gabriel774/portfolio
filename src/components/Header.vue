<template>
  <div>
    <div
      id="header"
      :style="{ 'background-color': background, color: fontColor }"
    >
      <div id="logo">Gabriel Santos</div>
      <div id="links">
        <span
          class="link"
          v-for="value in links"
          :key="value.name"
          @click="$vuetify.goTo(value.link)"
          >{{ value.name }}</span
        >
      </div>
      <div id="menu-mobile">
        <v-app-bar-nav-icon @click="drawer = true" :color="fontColor" text />
      </div>
    </div>
    <v-navigation-drawer v-model="drawer" fixed>
      <h1 class="homeTitle">Gabriel Santos</h1>
      <v-divider />
      <span
        class="link-mobile"
        v-for="value in links"
        :key="value.name"
        @click="[$vuetify.goTo(value.link), (drawer = false)]"
        flat
        >{{ value.name }}</span
      >
    </v-navigation-drawer>
  </div>
</template>

<script>
export default {
  computed: {
    background() {
      window.onload = () => {
        this.scroll = window.scrollY;
      };
      window.onscroll = () => {
        this.scroll = window.scrollY;
      };
      return this.scroll == 0 ? "transparent" : "#45aaf2";
    },
    fontColor() {
      window.onload = () => {
        this.scroll = window.scrollY;
      };
      window.onscroll = () => {
        this.scroll = window.scrollY;
      };
      return this.scroll == 0 ? "#45aaf2" : "white";
    },
  },
  data() {
    return {
      scroll: null,
      drawer: false,
      links: [
        { name: "Inicío", link: "#home" },
        { name: "Sobre Mim", link: "#aboutScroll" },
        { name: "Habilidades", link: "#skillsScroll" },
        { name: "Projetos", link: "#projectsScroll" },
      ],
    };
  },
  methods: {},
};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600&display=swap");
#header {
  position: fixed;
  top: 0px;
  width: 100%;
  display: flex;
  justify-content: space-between;
  align-items: center;
  flex-direction: row;
  height: 65px;
  color: #45aaf2;
  font-size: 18pt;
  transition: background-color 0.25s ease;
  font-family: montserrat;
  font-weight: 600;
}
#logo {
  margin-left: 15px;
}
.link {
  padding: 0px 10px;
  transition: all 0.25s ease;
  cursor: pointer;
}
.link:hover {
  text-decoration: underline;
}
.link-mobile {
  color: black;
  display: block;
  text-align: center;
  cursor: pointer;
  font-size: 18pt;
  user-select: none;
}
.link-mobile:hover {
  background: rgb(211, 211, 211);
}
#links {
  margin-right: 15px;
}
#menu-mobile {
  display: none;
  margin-right: 15px;
  color: #45aaf2;
}
.homeTitle {
  font-size: 35pt;
  margin: 0px;
  font-family: Montserrat;
  color: #45aaf2;
  text-align: center;
}
@media (max-width: 845px) {
  #links {
    display: none;
  }
  #menu-mobile {
    display: initial;
  }
}
</style>