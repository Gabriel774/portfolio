<template>
  <a
    class="project"
    :href="project.link"
    :style="{ background: project.background }"
    style="text-decoration: none; color: initial; overflow: none"
    target="_blank"
  >
    <h1 style="user-select: none" class="minor-font" v-html="project.name" />
  </a>
</template>

<script>
export default {
  props: ["project"],
};
</script>

<style>
.project {
  width: 420px;
  height: 110px;
  font-size: 16pt;
  background: tomato;
  border-radius: 10px;
  display: flex;
  justify-content: center;
  align-items: center;
  transition: transform 0.2s ease;
  cursor: pointer;
  overflow: none;
  margin: 10px;
  margin-bottom: 30px;
}
.project:hover {
  transform: translateY(-15px);
}
.font-mdm {
  font-size: 17.2pt;
}
@media (max-width: 720px) {
  .project:hover {
    transform: none;
  }
}
@media (max-width: 430px) {
  .project {
    width: 100%;
  }
  .minor-font {
    font-size: 22pt;
  }
  .font-mdm {
    font-size: 11pt;
  }
}
@media (max-width: 308px) {
  .minor-font {
    font-size: 16pt;
  }
  .font-mdm {
    font-size: 8pt;
  }
}
</style>