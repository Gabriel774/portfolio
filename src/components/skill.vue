<template>
  <div class="skill mt-12">
    <div class="skill-name">
      <img class="img-skill" :src="skillProp.logo" />
      <p :style="{ color: skillProp.color }" class="skill-name-value ml-2">
        {{ skillProp.name }}
      </p>
    </div>
    <v-progress-linear
      height="15"
      class="skill-level"
      :color="skillProp.color"
      :value="skillProp.value"
    />
  </div>
</template>

<script>
export default {
  props: ["skillProp"],
};
</script>

<style scoped>
.skill {
  display: flex;
  justify-content: space-between;
  min-height: 45px;
  align-items: center;
  margin: 0px 10%;
}
.skill-level {
  width: 500px;
}

.img-skill {
  width: 60px;
  height: 55px;
}
.skill-name {
  display: flex;
}
.skill-name-value {
  font-size: 28pt;
}
@media (max-width: 1264px) {
  .skill {
    flex-direction: column;
  }
  .skill-level {
    width: 95%;
  }
}
@media (max-width: 255px) {
  .skill-name-value {
    font-size: 20pt;
  }
}
</style>