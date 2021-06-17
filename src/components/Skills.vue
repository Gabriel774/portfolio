<template>
  <div id="skills" class="mt-12 container">
    <v-row></v-row>
    <h1 class="titleSection">Habilidades</h1>
    <h1 class="subTitleSection" style="margin-top: 20px">Tecnologias</h1>
    <Skill v-for="skill in skills" :key="skill.name" :skillProp="skill" />
    <h1 class="subTitleSection" style="margin-top: 50px">Ferramentas</h1>
    <Skill v-for="tool in tools" :key="tool.name" :skillProp="tool" />
  </div>
</template>

<script>
import Skill from "./skill.vue";
export default {
  components: { Skill },
  data() {
    return {
      skills: [
        {
          name: "HTML 5",
          logo: require("../assets/img/html5-logo-9.png"),
          color: "#EF642A",
          value: 100,
        },
        {
          name: "CSS 3",
          logo: require("../assets/img/css.png"),
          color: "#039BE5",
          value: 95,
        },
        {
          name: "JavaScript",
          logo: require("../assets/img/javascript.png"),
          color: "#fbc531",
          value: 97,
        },
        {
          name: "VueJS",
          logo: require("../assets/img/Vuejs.png"),
          color: "#3FB984",
          value: 92,
        },
        {
          name: "ReactJS",
          logo: require("../assets/img/react-logo-removebg-preview.png"),
          color: "#05A5D1",
          value: 75,
        },
        {
          name: "PHP",
          logo: require("../assets/img/php-logo.jpg"),
          color: "#6B7EB8",
          value: 67,
        },
        {
          name: "MySQL",
          logo: require("../assets/img/download__1_-removebg-preview.png"),
          color: "#217599",
          value: 65,
        },
      ],
      tools: [
        {
          name: "Visual Studio Code",
          logo: require("../assets/img/1024px-Visual_Studio_Code_1.35_icon.svg.png"),
          color: "#36A9F2",
          value: 100,
        },
        {
          name: "Adobe Photoshop",
          logo: require("../assets/img/1200px-Adobe_Photoshop_CC_icon.svg.png"),
          color: "#001833",
          value: 75,
        },
        {
          name: "Adobe Illustrator",
          logo: require("../assets/img/Adobe_Illustrator-logo-.png"),
          color: "#300000",
          value: 60,
        },
      ],
    };
  },
};
</script>

<style>
.subTitleSection {
  font-size: 32pt;
  text-align: center;
  color: #45aaf2;
}
@media (max-width: 300px) {
  .subTitleSection {
    font-size: 21pt;
    text-align: center;
    color: #45aaf2;
  }
}
</style>