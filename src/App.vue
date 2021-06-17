<template>
  <v-app id="app">
    <Home />
    <v-row />
    <div id="aboutScroll" />
    <About />
    <div id="skillsScroll" />
    <v-divider class="mt-6" />
    <Skills />
    <div id="projectsScroll" />
    <v-divider class="mt-6" />
    <Projects />
    <Footer />
    <transition name="fade" appear>
      <Header />
    </transition>
  </v-app>
</template>

<script>
import Header from "./components/Header.vue";
import Home from "./components/Home.vue";
import About from "./components/About.vue";
import Skills from "./components/Skills.vue";
import Projects from "./components/Projects.vue";
import Footer from "./components/Footer.vue";
export default {
  name: "App",
  components: {
    Home,
    Header,
    About,
    Skills,
    Projects,
    Footer,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Source+Sans+Pro:wght@400;700&display=swap");

body {
  margin: 0;
  padding: 0;
}
::-webkit-scrollbar {
  width: 11px;
}

::-webkit-scrollbar:hover {
  background-image: rgba(0, 0, 0, 0.445);
}

::-webkit-scrollbar-thumb {
  background-color: rgba(117, 117, 117, 0.377);
}

::-webkit-scrollbar-thumb:hover {
  background-color: rgba(105, 105, 105, 0.514);
}

::-webkit-scrollbar-thumb:active,
::-webkit-scrollbar-thumb:hover:active {
  background-color: rgba(78, 78, 78, 0.678);
}

::selection {
  background: #2c3e50;
  color: white;
}
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  font-family: "Source Sans Pro";
}
.fade-enter-active {
  animation: fade 1s ease;
}
.titleSection {
  text-align: center;
  font-size: 39pt;
  color: #45aaf2;
}
@keyframes fade {
  from {
    opacity: 0;
  }
}
@media (max-width: 300px) {
  .titleSection {
    font-size: 29pt;
  }
}
</style>