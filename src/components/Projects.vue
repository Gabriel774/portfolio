<template>
  <div id="projects" class="mt-12 container">
    <h1 class="titleSection">Projetos</h1>
    <h2 style="text-align: center; margin-bottom: 30px">
      Estes são alguns dos meus projetos, você pode conferir estes e outros no
      <a href="https://github.com/gabriel774" target="_blank">meu GitHub</a>.
      (Projetos como Nuntium e ProcuraBooks são de marcas fictícias, e foram
      feitos somente para fins de estudo/treino)
    </h2>
    <div id="projects-container">
      <Project
        v-for="project in projects"
        :key="project.name"
        :project="project"
      />
    </div>
  </div>
</template>

<script>
import Project from "./Project.vue";
export default {
  components: { Project },
  data() {
    return {
      projects: [
        {
          name: '<span style="color: white; font-family: Oswald; font-weight: 400"><span style="color: #3498DB">N</span>UNTIUM</span>',
          background: "#2b2d42",
          link: "https://gabriel774.github.io/nuntium",
        },
        {
          name: '<span style="font-family: Major Mono Display,monospace; @media (max-width: 430px) { font-size: 5pt }">ProcuraBooks</span>',
          background: "#ff8331",
          link: "https://gabriel774.github.io/ProcuraBooks",
        },
        {
          name: '<span style="font-family: Roboto Mono, monospace; color:white;">CALCULADORA<span style="color: #41B883">VUE</span></span>',
          background: "linear-gradient(to right, #283E51, #4B79A1)",
          link: "https://gabriel774.github.io/calculadora-vue",
        },
        {
          name: '<span style="font-family: Handlee; color:white; font-weight: 400;">Minhas<span style="color: #3498DB">Tarefas</span></span>',
          background:
            "linear-gradient(to right, rgb(22, 34, 42), rgb(58, 96, 115))",
          link: "https://gabriel774.github.io/minhas-tarefas",
        },
        {
          name: '<span style="font-family: Russo One, sans-serif; font-weight: 400; color: white">CRONÔMETRO</span>',
          background: "#3B3B98",
          link: "https://gabriel774.github.io/Cronometro",
        },
        {
          name: `<span class="font-mdm" style="font-family: 'Press Start 2P', cursive; font-weight:400; color: black;">MatadorDeMonstros</span>`,
          background: "#e74c3c",
          link: "https://gabriel774.github.io/MatadorDeMonstros",
        },
      ],
    };
  },
};
</script>

<style scoped>
#projects-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
}
</style>