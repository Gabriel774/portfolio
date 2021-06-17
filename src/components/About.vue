<template>
  <div id="about" class="container mt-12">
    <h1 class="titleSection">Sobre Mim</h1>
    <div class="about-container mt-7">
      <img class="profile-pic" src="../assets/img/eu.jpg" />
      <div class="about-text">
        <h1 class="text-title">Gabriel Santos de Sousa</h1>
        <p class="text-sub">
          Sou apaixonado por tecnologia em geral desde que me conheço por gente,
          e com programação não foi direfente, comecei de forma despretenciosa
          mas logo entrei de cabeça nesse mundo, tento estudar e aprimorar meus
          conhecimentos diariamente para criar aplicações cada vez melhores.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
#about {
  border-radius: 10px;
  padding: 0px 30px;
}
.profile-pic {
  border-radius: 50%;
  width: 360px;
  height: 360px;
  transition: box-shadow 0.5s ease;
}
.about-container {
  display: flex;
  justify-content: space-around;
}
.about-text {
  display: flex;
  flex-direction: column;
  max-width: 50%;
}
.text-sub {
  font-size: 18pt;
  text-align: center;
}
.text-title {
  text-align: center;
  font-size: 32pt;
}
@media (max-width: 845px) {
  .about-container {
    flex-direction: column;
    justify-content: center;
    align-items: center;
  }
  .about-text {
    max-width: none;
  }
}
@media (max-width: 365px) {
  .profile-pic {
    width: 200px;
    height: 200px;
  }
}
@media (min-width: 1850px) {
  .profile-pic {
    width: 500px;
    height: 500px;
  }
  .text-sub {
    font-size: 28pt;
  }
  .titleSection {
    font-size: 44pt;
  }
  .text-title {
    font-size: 40pt;
  }
}
@media (min-width: 1440px) {
  .profile-pic {
    width: 450px;
    height: 450px;
  }
  .text-sub {
    font-size: 22pt;
  }
  .titlesection {
    font-size: 40pt;
  }
  .text-title {
    font-size: 38pt;
  }
}
</style>