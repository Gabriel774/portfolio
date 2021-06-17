<template>
  <div id="home">
    <transition-group name="fadeIn" appear>
      <h1 class="homeTitle" key="title">Gabriel Santos</h1>
      <h2 class="subTitle" key="subTitle">Front-End Developer</h2>
      <div class="social" key="social">
        <a href="https://github.com/Gabriel774" target="_blank">
          <abbr title="GitHub">
            <img
              class="icon"
              src="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZlcnNpb249IjEuMSIgeG1sbnM6eGxpbms9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkveGxpbmsiIHhtbG5zOnN2Z2pzPSJodHRwOi8vc3ZnanMuY29tL3N2Z2pzIiB3aWR0aD0iNTEyIiBoZWlnaHQ9IjUxMiIgeD0iMCIgeT0iMCIgdmlld0JveD0iMCAwIDUxMiA1MTIiIHN0eWxlPSJlbmFibGUtYmFja2dyb3VuZDpuZXcgMCAwIDUxMiA1MTIiIHhtbDpzcGFjZT0icHJlc2VydmUiIGNsYXNzPSIiPjxnPgo8ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgoJPGc+CgkJPHBhdGggZD0iTTI1NS45NjgsNS4zMjlDMTE0LjYyNCw1LjMyOSwwLDEyMC40MDEsMCwyNjIuMzUzYzAsMTEzLjUzNiw3My4zNDQsMjA5Ljg1NiwxNzUuMTA0LDI0My44NzIgICAgYzEyLjgsMi4zNjgsMTcuNDcyLTUuNTY4LDE3LjQ3Mi0xMi4zODRjMC02LjExMi0wLjIyNC0yMi4yNzItMC4zNTItNDMuNzEyYy03MS4yLDE1LjUyLTg2LjI0LTM0LjQ2NC04Ni4yNC0zNC40NjQgICAgYy0xMS42MTYtMjkuNjk2LTI4LjQxNi0zNy42LTI4LjQxNi0zNy42Yy0yMy4yNjQtMTUuOTM2LDEuNzI4LTE1LjYxNiwxLjcyOC0xNS42MTZjMjUuNjk2LDEuODI0LDM5LjIsMjYuNDk2LDM5LjIsMjYuNDk2ICAgIGMyMi44NDgsMzkuMjY0LDU5LjkzNiwyNy45MzYsNzQuNTI4LDIxLjM0NGMyLjMwNC0xNi42MDgsOC45MjgtMjcuOTM2LDE2LjI1Ni0zNC4zNjggICAgYy01Ni44MzItNi40OTYtMTE2LjYwOC0yOC41NDQtMTE2LjYwOC0xMjcuMDA4YzAtMjguMDY0LDkuOTg0LTUxLjAwOCwyNi4zNjgtNjguOTkyYy0yLjY1Ni02LjQ5Ni0xMS40MjQtMzIuNjQsMi40OTYtNjggICAgYzAsMCwyMS41MDQtNi45MTIsNzAuNCwyNi4zMzZjMjAuNDE2LTUuNjk2LDQyLjMwNC04LjU0NCw2NC4wOTYtOC42NGMyMS43MjgsMC4xMjgsNDMuNjQ4LDIuOTQ0LDY0LjA5Niw4LjY3MiAgICBjNDguODY0LTMzLjI0OCw3MC4zMzYtMjYuMzM2LDcwLjMzNi0yNi4zMzZjMTMuOTUyLDM1LjM5Miw1LjE4NCw2MS41MDQsMi41Niw2OGMxNi40MTYsMTcuOTg0LDI2LjMwNCw0MC45MjgsMjYuMzA0LDY4Ljk5MiAgICBjMCw5OC43Mi01OS44NCwxMjAuNDQ4LTExNi44NjQsMTI2LjgxNmM5LjE4NCw3LjkzNiwxNy4zNzYsMjMuNjE2LDE3LjM3Niw0Ny41ODRjMCwzNC4zNjgtMC4zMiw2Mi4wOC0wLjMyLDcwLjQ5NiAgICBjMCw2Ljg4LDQuNjA4LDE0Ljg4LDE3LjYsMTIuMzUyQzQzOC43Miw0NzIuMTQ1LDUxMiwzNzUuODU3LDUxMiwyNjIuMzUzQzUxMiwxMjAuNDAxLDM5Ny4zNzYsNS4zMjksMjU1Ljk2OCw1LjMyOXoiIGZpbGw9IiM0NWFhZjIiIGRhdGEtb3JpZ2luYWw9IiMwMDAwMDAiIHN0eWxlPSIiIGNsYXNzPSIiPjwvcGF0aD4KCTwvZz4KPC9nPgo8ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgo8L2c+CjxnIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjwvZz4KPGcgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPC9nPgo8ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgo8L2c+CjxnIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjwvZz4KPGcgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPC9nPgo8ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgo8L2c+CjxnIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjwvZz4KPGcgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPC9nPgo8ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgo8L2c+CjxnIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjwvZz4KPGcgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPC9nPgo8ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgo8L2c+CjxnIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjwvZz4KPGcgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPC9nPgo8L2c+PC9zdmc+"
            />
          </abbr>
        </a>
        <a
          href="https://www.linkedin.com/in/gabriel-santos-de-sousa-4b72aa208/"
          target="_blank"
        >
          <abbr title="Linkedin">
            <img
              class="icon"
              src="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZlcnNpb249IjEuMSIgeG1sbnM6eGxpbms9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkveGxpbmsiIHhtbG5zOnN2Z2pzPSJodHRwOi8vc3ZnanMuY29tL3N2Z2pzIiB3aWR0aD0iNTEyIiBoZWlnaHQ9IjUxMiIgeD0iMCIgeT0iMCIgdmlld0JveD0iMCAwIDUxMiA1MTIiIHN0eWxlPSJlbmFibGUtYmFja2dyb3VuZDpuZXcgMCAwIDUxMiA1MTIiIHhtbDpzcGFjZT0icHJlc2VydmUiIGNsYXNzPSIiPjxnPjxwYXRoIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyIgZD0ibTI1NiAwYy0xNDEuMzYzMjgxIDAtMjU2IDExNC42MzY3MTktMjU2IDI1NnMxMTQuNjM2NzE5IDI1NiAyNTYgMjU2IDI1Ni0xMTQuNjM2NzE5IDI1Ni0yNTYtMTE0LjYzNjcxOS0yNTYtMjU2LTI1NnptLTc0LjM5MDYyNSAzODdoLTYyLjM0NzY1NnYtMTg3LjU3NDIxOWg2Mi4zNDc2NTZ6bS0zMS4xNzE4NzUtMjEzLjE4NzVoLS40MDYyNWMtMjAuOTIxODc1IDAtMzQuNDUzMTI1LTE0LjQwMjM0NC0zNC40NTMxMjUtMzIuNDAyMzQ0IDAtMTguNDA2MjUgMTMuOTQ1MzEzLTMyLjQxMDE1NiAzNS4yNzM0MzctMzIuNDEwMTU2IDIxLjMyODEyNiAwIDM0LjQ1MzEyNiAxNC4wMDM5MDYgMzQuODU5Mzc2IDMyLjQxMDE1NiAwIDE4LTEzLjUzMTI1IDMyLjQwMjM0NC0zNS4yNzM0MzggMzIuNDAyMzQ0em0yNTUuOTg0Mzc1IDIxMy4xODc1aC02Mi4zMzk4NDR2LTEwMC4zNDc2NTZjMC0yNS4yMTg3NS05LjAyNzM0My00Mi40MTc5NjktMzEuNTg1OTM3LTQyLjQxNzk2OS0xNy4yMjI2NTYgMC0yNy40ODA0NjkgMTEuNjAxNTYzLTMxLjk4ODI4MiAyMi44MDA3ODEtMS42NDg0MzcgNC4wMDc4MTMtMi4wNTA3ODEgOS42MDkzNzUtMi4wNTA3ODEgMTUuMjE0ODQ0djEwNC43NWgtNjIuMzQzNzVzLjgxNjQwNy0xNjkuOTc2NTYyIDAtMTg3LjU3NDIxOWg2Mi4zNDM3NXYyNi41NTg1OTRjOC4yODUxNTctMTIuNzgxMjUgMjMuMTA5Mzc1LTMwLjk2MDkzNyA1Ni4xODc1LTMwLjk2MDkzNyA0MS4wMTk1MzEgMCA3MS43NzczNDQgMjYuODA4NTkzIDcxLjc3NzM0NCA4NC40MjE4NzR6bTAgMCIgZmlsbD0iIzQ1YWFmMiIgZGF0YS1vcmlnaW5hbD0iIzAwMDAwMCIgc3R5bGU9IiI+PC9wYXRoPjwvZz48L3N2Zz4="
            />
          </abbr>
        </a>
        <a href="mailto:gabrielsantossousa774@gmail.com">
          <abbr title="E-mail">
            <img class="icon" src="../assets/img/email.png" />
          </abbr>
        </a>
      </div>
    </transition-group>
    <transition name="fade" appear>
      <img
        class="arrow"
        key="arrow"
        src="data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZlcnNpb249IjEuMSIgeG1sbnM6eGxpbms9Imh0dHA6Ly93d3cudzMub3JnLzE5OTkveGxpbmsiIHhtbG5zOnN2Z2pzPSJodHRwOi8vc3ZnanMuY29tL3N2Z2pzIiB3aWR0aD0iNTEyIiBoZWlnaHQ9IjUxMiIgeD0iMCIgeT0iMCIgdmlld0JveD0iMCAwIDQ5MS45OTYgNDkxLjk5NiIgc3R5bGU9ImVuYWJsZS1iYWNrZ3JvdW5kOm5ldyAwIDAgNTEyIDUxMiIgeG1sOnNwYWNlPSJwcmVzZXJ2ZSIgY2xhc3M9IiI+PGc+CjxnIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+Cgk8Zz4KCQk8cGF0aCBkPSJNNDg0LjEzMiwxMjQuOTg2bC0xNi4xMTYtMTYuMjI4Yy01LjA3Mi01LjA2OC0xMS44Mi03Ljg2LTE5LjAzMi03Ljg2Yy03LjIwOCwwLTEzLjk2NCwyLjc5Mi0xOS4wMzYsNy44NmwtMTgzLjg0LDE4My44NDggICAgTDYyLjA1NiwxMDguNTU0Yy01LjA2NC01LjA2OC0xMS44Mi03Ljg1Ni0xOS4wMjgtNy44NTZzLTEzLjk2OCwyLjc4OC0xOS4wMzYsNy44NTZsLTE2LjEyLDE2LjEyOCAgICBjLTEwLjQ5NiwxMC40ODgtMTAuNDk2LDI3LjU3MiwwLDM4LjA2bDIxOS4xMzYsMjE5LjkyNGM1LjA2NCw1LjA2NCwxMS44MTIsOC42MzIsMTkuMDg0LDguNjMyaDAuMDg0ICAgIGM3LjIxMiwwLDEzLjk2LTMuNTcyLDE5LjAyNC04LjYzMmwyMTguOTMyLTIxOS4zMjhjNS4wNzItNS4wNjQsNy44NTYtMTIuMDE2LDcuODY0LTE5LjIyNCAgICBDNDkxLjk5NiwxMzYuOTAyLDQ4OS4yMDQsMTMwLjA0Niw0ODQuMTMyLDEyNC45ODZ6IiBmaWxsPSIjNDVhYWYyIiBkYXRhLW9yaWdpbmFsPSIjMDAwMDAwIiBzdHlsZT0iIiBjbGFzcz0iIj48L3BhdGg+Cgk8L2c+CjwvZz4KPGcgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPC9nPgo8ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgo8L2c+CjxnIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjwvZz4KPGcgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPC9nPgo8ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgo8L2c+CjxnIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjwvZz4KPGcgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPC9nPgo8ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgo8L2c+CjxnIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjwvZz4KPGcgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPC9nPgo8ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgo8L2c+CjxnIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjwvZz4KPGcgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4KPC9nPgo8ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciPgo8L2c+CjxnIHhtbG5zPSJodHRwOi8vd3d3LnczLm9yZy8yMDAwL3N2ZyI+CjwvZz4KPC9nPjwvc3ZnPg=="
        @click="$vuetify.goTo('#aboutScroll')"
      />
    </transition>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Roboto+Condensed&display=swap");

#home {
  width: 100%;
  height: 100vh;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  color: #45aaf2;
  text-align: center;
  position: relative;
  background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' version='1.1' xmlns:xlink='http://www.w3.org/1999/xlink' xmlns:svgjs='http://svgjs.com/svgjs' width='1440' height='560' preserveAspectRatio='none' viewBox='0 0 1440 560'%3e%3cg mask='url(%26quot%3b%23SvgjsMask1002%26quot%3b)' fill='none'%3e%3crect width='1440' height='560' x='0' y='0' fill='url(%23SvgjsLinearGradient1003)'%3e%3c/rect%3e%3cpath d='M287.868732594124 508.040445717545L401.56279200139517 502.08199254633575 395.6043388301859 388.38793313906456 281.91027942291475 394.3463863102739z' fill='rgba(28%2c 83%2c 142%2c 0.4)' class='triangle-float3'%3e%3c/path%3e%3cpath d='M294.834%2c355.575C330.991%2c356.856%2c362.543%2c330.449%2c377.945%2c297.711C391.433%2c269.04%2c379.676%2c237.321%2c363.199%2c210.257C347.566%2c184.58%2c324.888%2c161.897%2c294.834%2c161.2C263.733%2c160.479%2c235.975%2c179.826%2c220.75%2c206.955C205.851%2c233.502%2c207.755%2c264.917%2c221.336%2c292.162C236.808%2c323.2%2c260.175%2c354.347%2c294.834%2c355.575' fill='rgba(28%2c 83%2c 142%2c 0.4)' class='triangle-float3'%3e%3c/path%3e%3cpath d='M376.334%2c650.77C413.849%2c647.539%2c445.358%2c624.395%2c463.366%2c591.326C480.547%2c559.777%2c478.682%2c523.314%2c463.461%2c490.774C444.982%2c451.267%2c419.889%2c407.551%2c376.334%2c405.262C330.329%2c402.844%2c294.784%2c440.8%2c271.757%2c480.7C248.738%2c520.586%2c234.66%2c569.717%2c258.782%2c608.946C282.131%2c646.918%2c331.922%2c654.595%2c376.334%2c650.77' fill='rgba(28%2c 83%2c 142%2c 0.4)' class='triangle-float2'%3e%3c/path%3e%3cpath d='M620.8826514414715 110.0448465980971L680.8789321740185 186.8365840844273 757.6706696603486 126.84030335188034 697.6743889278017 50.04856586555013z' fill='rgba(28%2c 83%2c 142%2c 0.4)' class='triangle-float3'%3e%3c/path%3e%3cpath d='M982.632%2c465.136C1024.014%2c465.049%2c1059.822%2c439.449%2c1080.92%2c403.849C1102.489%2c367.455%2c1108.97%2c322.988%2c1088.971%2c285.708C1067.915%2c246.458%2c1027.172%2c220.278%2c982.632%2c220.63C938.646%2c220.978%2c900.043%2c248.65%2c879.168%2c287.368C859.335%2c324.155%2c862.604%2c368.142%2c883.627%2c404.263C904.513%2c440.149%2c941.11%2c465.223%2c982.632%2c465.136' fill='rgba(28%2c 83%2c 142%2c 0.4)' class='triangle-float1'%3e%3c/path%3e%3cpath d='M1222.2964386843882 254.1851975603663L1311.2715428962938 331.53007564759247 1299.6413167716144 165.21009334846076z' fill='rgba(28%2c 83%2c 142%2c 0.4)' class='triangle-float2'%3e%3c/path%3e%3c/g%3e%3cdefs%3e%3cmask id='SvgjsMask1002'%3e%3crect width='1440' height='560' fill='white'%3e%3c/rect%3e%3c/mask%3e%3clinearGradient x1='15.28%25' y1='-39.29%25' x2='84.72%25' y2='139.29%25' gradientUnits='userSpaceOnUse' id='SvgjsLinearGradient1003'%3e%3cstop stop-color='%230e2a47' offset='0'%3e%3c/stop%3e%3cstop stop-color='%2300459e' offset='1'%3e%3c/stop%3e%3c/linearGradient%3e%3cstyle%3e %40keyframes float1 %7b 0%25%7btransform: translate(0%2c 0)%7d 50%25%7btransform: translate(-10px%2c 0)%7d 100%25%7btransform: translate(0%2c 0)%7d %7d .triangle-float1 %7b animation: float1 5s infinite%3b %7d %40keyframes float2 %7b 0%25%7btransform: translate(0%2c 0)%7d 50%25%7btransform: translate(-5px%2c -5px)%7d 100%25%7btransform: translate(0%2c 0)%7d %7d .triangle-float2 %7b animation: float2 4s infinite%3b %7d %40keyframes float3 %7b 0%25%7btransform: translate(0%2c 0)%7d 50%25%7btransform: translate(0%2c -10px)%7d 100%25%7btransform: translate(0%2c 0)%7d %7d .triangle-float3 %7b animation: float3 6s infinite%3b %7d %3c/style%3e%3c/defs%3e%3c/svg%3e");
  background-position: center;
  background-size: cover;
  background-attachment: fixed;
  font-family: "Roboto Condensed";
}
.homeTitle {
  font-size: 65pt;
  margin: 0px;
}
.subTitle {
  font-size: 26pt;
}
.img {
  width: 50px;
  padding: 10px;
}
.icon {
  width: 80px;
  padding: 10px;
  transition: transform 0.2s;
  cursor: pointer;
}
.icon:hover {
  transform: translateY(-10px);
}
.arrow {
  width: 70px;
  transition: transform 0.2s;
  cursor: pointer;
  position: absolute;
  bottom: 10px;
}
.arrow:hover {
  transform: translateY(10px);
}
.fadeIn-enter-active {
  animation: fadeIn 0.5s ease;
}
.fade-enter-active {
  animation: fade 1s ease;
}
@keyframes fadeIn {
  from {
    transform: translateY(50px);
    opacity: 0;
  }
}
@keyframes fade {
  from {
    opacity: 0;
  }
}
@media (min-width: 1800px) {
  .homeTitle {
    font-size: 78pt;
    line-height: 90px;
  }
  .subTitle {
    font-size: 38pt;
  }
  .icon {
    width: 110px;
  }
}
@media (max-width: 865px) {
  .homeTitle {
    font-size: 68pt;
    line-height: 90px;
  }
  .subTitle {
    font-size: 24pt;
  }
  #home {
    background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' version='1.1' xmlns:xlink='http://www.w3.org/1999/xlink' xmlns:svgjs='http://svgjs.com/svgjs' width='845' height='560' preserveAspectRatio='none' viewBox='0 0 845 560'%3e%3cg mask='url(%26quot%3b%23SvgjsMask1142%26quot%3b)' fill='none'%3e%3crect width='845' height='560' x='0' y='0' fill='url(%23SvgjsLinearGradient1143)'%3e%3c/rect%3e%3cpath d='M150.341%2c394.394C173.56%2c394.923%2c196.516%2c384.872%2c208.23%2c364.818C220.036%2c344.606%2c218.818%2c318.837%2c205.863%2c299.34C194.081%2c281.608%2c171.631%2c277.558%2c150.341%2c277.695C129.364%2c277.83%2c107.259%2c282.32%2c96.047%2c300.049C84.163%2c318.841%2c85.76%2c343.008%2c96.85%2c362.279C107.968%2c381.598%2c128.057%2c393.886%2c150.341%2c394.394' fill='rgba(28%2c 83%2c 142%2c 0.4)' class='triangle-float2'%3e%3c/path%3e%3cpath d='M216.792733279519 314.3135602141797L307.6105163487722 307.96296217636944 252.6757277574303 174.91158659139475z' fill='rgba(28%2c 83%2c 142%2c 0.4)' class='triangle-float2'%3e%3c/path%3e%3cpath d='M406.05851288827546 63.44847997997957L451.8623462345594 110.87973789786793 500.10731643825 18.458358919497776z' fill='rgba(28%2c 83%2c 142%2c 0.4)' class='triangle-float3'%3e%3c/path%3e%3cpath d='M478.676%2c600.757C517.65%2c602.875%2c553.095%2c577.547%2c571.488%2c543.12C588.9%2c510.53%2c582.754%2c472.11%2c564.601%2c439.926C546.069%2c407.071%2c516.382%2c377.499%2c478.676%2c378.57C442.222%2c379.606%2c416.983%2c411.892%2c400.812%2c444.58C386.662%2c473.184%2c387.596%2c505.339%2c401.835%2c533.899C418.071%2c566.465%2c442.341%2c598.782%2c478.676%2c600.757' fill='rgba(28%2c 83%2c 142%2c 0.4)' class='triangle-float2'%3e%3c/path%3e%3cpath d='M459.7825304206952 497.8834226920228L572.6046325811208 445.2736124454707 407.1727201741431 385.06132053159723z' fill='rgba(28%2c 83%2c 142%2c 0.4)' class='triangle-float3'%3e%3c/path%3e%3cpath d='M414.1026826331133 199.57032093003943L306.78353427114564 76.11376316456749 183.3269765056737 183.43291152653512 290.6461248676414 306.8894692920071z' fill='rgba(28%2c 83%2c 142%2c 0.4)' class='triangle-float3'%3e%3c/path%3e%3c/g%3e%3cdefs%3e%3cmask id='SvgjsMask1142'%3e%3crect width='845' height='560' fill='white'%3e%3c/rect%3e%3c/mask%3e%3clinearGradient x1='8.43%25' y1='-12.72%25' x2='91.57%25' y2='112.72%25' gradientUnits='userSpaceOnUse' id='SvgjsLinearGradient1143'%3e%3cstop stop-color='%230e2a47' offset='0'%3e%3c/stop%3e%3cstop stop-color='%2300459e' offset='1'%3e%3c/stop%3e%3c/linearGradient%3e%3cstyle%3e %40keyframes float1 %7b 0%25%7btransform: translate(0%2c 0)%7d 50%25%7btransform: translate(-10px%2c 0)%7d 100%25%7btransform: translate(0%2c 0)%7d %7d .triangle-float1 %7b animation: float1 5s infinite%3b %7d %40keyframes float2 %7b 0%25%7btransform: translate(0%2c 0)%7d 50%25%7btransform: translate(-5px%2c -5px)%7d 100%25%7btransform: translate(0%2c 0)%7d %7d .triangle-float2 %7b animation: float2 4s infinite%3b %7d %40keyframes float3 %7b 0%25%7btransform: translate(0%2c 0)%7d 50%25%7btransform: translate(0%2c -10px)%7d 100%25%7btransform: translate(0%2c 0)%7d %7d .triangle-float3 %7b animation: float3 6s infinite%3b %7d %3c/style%3e%3c/defs%3e%3c/svg%3e");
    background-attachment: initial;
  }
}
@media (max-width: 365px) {
  .homeTitle {
    font-size: 48pt;
    line-height: 90px;
  }
}
</style>