<template>
  <div>
    <div class="relative" style="z-index: 10">
      <nav class="db dt-l w-100 border-box pa3 ph5-l bg-black">
        <a class="db dtc-l v-mid link dim w-100 w-25-l tc tl-l mb2 mb0-l" href="https://it.wikipedia.org/wiki/Gemelli_(costellazione)" title="Gemini">
          <img class="dib w2 h2 ba b--white-20 bw3" src="~/static/200px-Gemini2.jpg">
        </a>
        <div class="db dtc-l v-mid w-100 w-75-l tc tr-l">
          <NuxtLink class="link dim white f6 f5-l fw6 dib mr3 mr4-l" to="/chisiamo" title="Chi siamo">Chi siamo</NuxtLink>
          <NuxtLink class="link dim white f6 f5-l fw6 dib mr3 mr4-l" to="/dovesiamo" title="Dove siamo">Dove siamo</NuxtLink>
          <NuxtLink class="link dim white f6 f5-l fw6 dib mr3 mr4-l" to="/perche" title="Perchè">Perchè</NuxtLink>
          <NuxtLink class="link dim white f6 f5-l fw6 dib" to="/contatti" title="Contatti">Contatti</NuxtLink>
        </div>
      </nav>
    </div>

    <div class="body vh-100">
      <div>
        <div class="stars">
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
            <div class="star"></div>
        </div>
      </div>

      <div class="flex flex-wrap justify-around w-80 vh-75 center items-center relative">
        <h1 class="titolo w-100 f-headline-l lh-solid-l f2 lh-title tc">Non Facciamone Un Dramma</h1>
        <!-- titolo colorato -->
        <!-- <h1 class="titolo w-100 f-headline-l lh-solid-l f2 lh-title tc">
          <span class="red">N</span><span class="white">o</span><span class="green">n</span>
          <span class="orange">Fa</span><span class="purple">cci</span><span class="yellow">amone</span>
          <span class="white">Un</span>
          <span class="dark-red">Dr</span><span class="white">a</span><span class="dark-green">mma</span>
        </h1> -->

        <NuxtLink  class="mdma cover w-80 w-30-l w-40-m db bb ba bw2 b--dark-red pa2 br4 link dim" :to="{ name: 'mdma' }">
          <h1 class="tc white">MDMA</h1>
          <h3 class="tc white">Mai Dire Mi Arrendo</h3>
        </NuxtLink>
        <NuxtLink  class="ndi cover w-80 w-30-l w-40-m db bb ba bw2 b--dark-blue pa2 br4 link dim" :to="{ name: 'ndi' }">
          <h1 class="tc white">NDI</h1>
          <h3 class="tc white">Nel Dominio dell'Incerto</h3>
        </NuxtLink>
      </div>

    </div>
  </div>

</template>

<script>
export default {
}
</script>

<style scoped>
/*
.dark-red { color: var(--dark-red); }
.red { color: var(--red); }
.orange { color: var(--orange); }
.gold { color: var(--gold); }
.yellow { color: var(--yellow); }
.purple { color: var(--purple); }
.light-purple { color: var(--light-purple); }
.hot-pink { color:  var(--hot-pink); }
.dark-pink { color: var(--dark-pink); }
.pink { color: var(--pink); }
.dark-green { color: var(--dark-green); }
.green { color: var(--green); }
.navy { color: var(--navy); }
.dark-blue { color: var(--dark-blue); }
.blue { color: var(--blue); }
.light-blue { color: var(--light-blue); }
.lightest-blue { color: var(--lightest-blue); }
.washed-blue { color: var(--washed-blue); }
.washed-green { color: var(--washed-green); }
.washed-yellow { color: var(--washed-yellow); }
.light-pink { color: var(--light-pink); }
.light-yellow { color: var(--light-yellow); }
.light-red { color: var(--light-red); }
*/

/* definiti in assets/font.css
font-family: "Lobster";
font-family: "AbrilFatface";
font-family: "Curely";
font-family: "LibreBaskerville-Regular";
font-family: "LibreBaskerville-Bold";
font-family: "LibreBaskerville-Italic";
font-family: "MerryChristmasFlake";
font-family: "MerryChristmasStar";
*/

.mdma {
  background-image: url("~/static/teatro.png");
}

.ndi {
  /* background-image: url("~/static/dom-j-ndi.jpg"); */
  background-image: url("~/static/pexels-adrien-olichon-2387793.jpg");
}

.titolo {
  /* font-family: "Lobster"; */
  /* font-family: "AbrilFatface"; */
  /* font-family: "Curely"; */
  /* font-family: "LibreBaskerville-Regular"; */
  font-family: "LibreBaskerville-Bold";
  /* font-family: "LibreBaskerville-Italic"; */
  /* font-family: "MerryChristmasFlake"; */
  /* font-family: 'MerryChristmasStar'; */
  /* font-size: 10rem; */

  color: white;
  /* offset-x | offset-y | blur-radius | color */
  text-shadow: 4px 3px 2px black;
}


.body {
  display: flex;
  background: radial-gradient(ellipse at bottom, #154785 0%, #061258 100%);
  overflow: hidden;
}

.stars {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  transform: rotate(220deg);
}

.star {
  /* --star-color: var(--primary-color); */
  --star-color: white;
  --star-tail-length: 6em;
  --star-tail-height: 2px;
  --star-width: calc(var(--star-tail-length) / 6);
  --fall-duration: 9s;
  --tail-fade-duration: var(--fall-duration);
  position: absolute;
  top: var(--top-offset);
  left: 0;
  width: var(--star-tail-length);
  height: var(--star-tail-height);
  color: var(--star-color);
  background: linear-gradient(45deg, currentColor, transparent);
  border-radius: 50%;
  filter: drop-shadow(0 0 6px currentColor);
  transform: translate3d(110rem, 0, 0);
  animation: fall var(--fall-duration) var(--fall-delay) linear infinite, tail-fade var(--tail-fade-duration) var(--fall-delay) ease-out infinite;
}

/* @media screen and (max-width: 750px) {
  .star {
    animation: fall var(--fall-duration) var(--fall-delay) linear infinite;
  }
} */

.star:nth-child(1) {
  --star-tail-length: 6.33em;
  --top-offset: 77.66vh;
  --fall-duration: 8.929s;
  --fall-delay: 0s;
  color: red;
}
.star:nth-child(2) {
  --star-tail-length: 5.41em;
  --top-offset: 66.45vh;
  --fall-duration: 9.18s;
  --fall-delay: 7.533s;
  color: green;
}
.star:nth-child(3) {
  --star-tail-length: 7.13em;
  --top-offset: 3.73vh;
  --fall-duration: 9.095s;
  --fall-delay: 0.789s;
  color: darkgoldenrod;
}
.star:nth-child(4) {
  --star-tail-length: 5.45em;
  --top-offset: 32.81vh;
  --fall-duration: 8.353s;
  --fall-delay: 5.037s;
  color: darkorchid;
}
.star:nth-child(5) {
  --star-tail-length: 5.88em;
  --top-offset: 36.17vh;
  --fall-duration: 7.736s;
  --fall-delay: 5.525s;
  color: lightseagreen;
}
.star:nth-child(6) {
  --star-tail-length: 6.79em;
  --top-offset: 25.32vh;
  --fall-duration: 9.225s;
  --fall-delay: 0.885s;
  color: lightseagreen;
}
.star:nth-child(7) {
  --star-tail-length: 6.2em;
  --top-offset: 4.86vh;
  --fall-duration: 11.923s;
  --fall-delay: 5.795s;
  color: darkorchid;
}
.star:nth-child(8) {
  --star-tail-length: 6.15em;
  --top-offset: 57.05vh;
  --fall-duration: 11.167s;
  --fall-delay: 5.189s;
  color: darkgoldenrod;
}
.star:nth-child(9) {
  --star-tail-length: 5em;
  --top-offset: 49.36vh;
  --fall-duration: 8.569s;
  --fall-delay: 2.799s;
  color: green;
}
.star:nth-child(10) {
  --star-tail-length: 5.39em;
  --top-offset: 73.24vh;
  --fall-duration: 10.344s;
  --fall-delay: 1.651s;
  color: red;
}
.star:nth-child(11) {
  --star-tail-length: 7.35em;
  --top-offset: 10.55vh;
  --fall-duration: 10.43s;
  --fall-delay: 6.337s;
  color: rebeccapurple 
}
.star:nth-child(12) {
  --star-tail-length: 6.35em;
  --top-offset: 33.21vh;
  --fall-duration: 10.945s;
  --fall-delay: 5.627s;
  color: purple;
}
.star:nth-child(13) {
  --star-tail-length: 6.36em;
  --top-offset: 42.23vh;
  --fall-duration: 11.774s;
  --fall-delay: 1.363s;
  color: aliceblue;
}
.star:nth-child(14) {
  --star-tail-length: 7.48em;
  --top-offset: 75.23vh;
  --fall-duration: 6.267s;
  --fall-delay: 9.347s;
  color: aqua;
}
.star:nth-child(15) {
  --star-tail-length: 6.35em;
  --top-offset: 80.78vh;
  --fall-duration: 6.651s;
  --fall-delay: 1.815s;
  color: darkolivegreen;
}
.star:nth-child(16) {
  --star-tail-length: 6.35em;
  --top-offset: 8.05vh;
  --fall-duration: 8.329s;
  --fall-delay: 2.114s;
  /* color: purple; */
}
.star:nth-child(17) {
  --star-tail-length: 7.25em;
  --top-offset: 40.49vh;
  --fall-duration: 8.396s;
  --fall-delay: 6.142s;
  /* color: purple; */
}
.star:nth-child(18) {
  --star-tail-length: 5.46em;
  --top-offset: 95.83vh;
  --fall-duration: 11.761s;
  --fall-delay: 6.646s;
  /* color: purple; */
}
.star:nth-child(19) {
  --star-tail-length: 5em;
  --top-offset: 94.48vh;
  --fall-duration: 8.516s;
  --fall-delay: 0.167s;
  color: darkslateblue;
}
.star:nth-child(20) {
  --star-tail-length: 5.08em;
  --top-offset: 78.87vh;
  --fall-duration: 11.227s;
  --fall-delay: 5.692s;
  color: grey;
}
.star:nth-child(21) {
  --star-tail-length: 6.03em;
  --top-offset: 85.84vh;
  --fall-duration: 11.36s;
  --fall-delay: 5.168s;
  color: hotpink;
}
.star:nth-child(22) {
  --star-tail-length: 5.29em;
  --top-offset: 57.64vh;
  --fall-duration: 9.115s;
  --fall-delay: 2.797s;
  color: indigo;
}
.star:nth-child(23) {
  --star-tail-length: 6.35em;
  --top-offset: 43.62vh;
  --fall-duration: 10.774s;
  --fall-delay: 5.491s;
  color: lawngreen;
}
.star:nth-child(24) {
  --star-tail-length: 6.87em;
  --top-offset: 22.35vh;
  --fall-duration: 10.127s;
  --fall-delay: 5.213s;
    /* color: purple; */
}
.star:nth-child(25) {
  --star-tail-length: 5.42em;
  --top-offset: 54.72vh;
  --fall-duration: 6.673s;
  --fall-delay: 8.7s;
  /* color: purple; */
}
.star:nth-child(26) {
  --star-tail-length: 7.24em;
  --top-offset: 27.5vh;
  --fall-duration: 8.846s;
  --fall-delay: 2.344s;
  /* color: purple; */
}
.star:nth-child(27) {
  --star-tail-length: 6.57em;
  --top-offset: 22.88vh;
  --fall-duration: 9.115s;
  --fall-delay: 4.447s;
  color: lime;
}
.star:nth-child(28) {
  --star-tail-length: 5.53em;
  --top-offset: 1.9vh;
  --fall-duration: 6.646s;
  --fall-delay: 8.373s;
  color: navy;
}
.star:nth-child(29) {
  --star-tail-length: 7.18em;
  --top-offset: 19.8vh;
  --fall-duration: 7.207s;
  --fall-delay: 4.792s;
  color: olive;
}
.star:nth-child(30) {
  --star-tail-length: 6.6em;
  --top-offset: 43.88vh;
  --fall-duration: 7.643s;
  --fall-delay: 6.105s;
  color: powderblue;
}
.star:nth-child(31) {
  --star-tail-length: 6.53em;
  --top-offset: 30.25vh;
  --fall-duration: 9.293s;
  --fall-delay: 6.155s;
  /* color: purple; */
}
.star:nth-child(32) {
  --star-tail-length: 5.99em;
  --top-offset: 81.24vh;
  --fall-duration: 8.362s;
  --fall-delay: 0.347s;
  /* color: purple; */
}
.star:nth-child(33) {
  --star-tail-length: 5.86em;
  --top-offset: 22.7vh;
  --fall-duration: 9.923s;
  --fall-delay: 0.406s;
  /* color: purple; */
}
.star:nth-child(34) {
  --star-tail-length: 6.97em;
  --top-offset: 60.26vh;
  --fall-duration: 11.125s;
  --fall-delay: 5.097s;
  /* color: purple; */
}
.star:nth-child(35) {
  --star-tail-length: 5.79em;
  --top-offset: 30.42vh;
  --fall-duration: 7.24s;
  --fall-delay: 6.678s;
  color: rebeccapurple;
}
.star:nth-child(36) {
  --star-tail-length: 7.31em;
  --top-offset: 81.33vh;
  --fall-duration: 8.909s;
  --fall-delay: 5.177s;
}
.star:nth-child(37) {
  --star-tail-length: 6.62em;
  --top-offset: 23.15vh;
  --fall-duration: 9.898s;
  --fall-delay: 3.553s;
  color: seashell;
}
.star:nth-child(38) {
  --star-tail-length: 5.83em;
  --top-offset: 45.2vh;
  --fall-duration: 6.332s;
  --fall-delay: 0.396s;
  /* color: purple; */
}
.star:nth-child(39) {
  --star-tail-length: 5em;
  --top-offset: 32.44vh;
  --fall-duration: 9.059s;
  --fall-delay: 4.646s;
  color: silver;
}
.star:nth-child(40) {
  --star-tail-length: 5.79em;
  --top-offset: 13.99vh;
  --fall-duration: 7.657s;
  --fall-delay: 0.72s;
  color: skyblue;
}
.star:nth-child(41) {
  --star-tail-length: 6.71em;
  --top-offset: 32.83vh;
  --fall-duration: 7.894s;
  --fall-delay: 0.145s;
  /* color: purple; */
}
.star:nth-child(42) {
  --star-tail-length: 7.42em;
  --top-offset: 59.85vh;
  --fall-duration: 10.152s;
  --fall-delay: 1.281s;
  /* color: purple; */
}
.star:nth-child(43) {
  --star-tail-length: 6.27em;
  --top-offset: 92.53vh;
  --fall-duration: 7.167s;
  --fall-delay: 6.359s;
  color: slategrey;
}
.star:nth-child(44) {
  --star-tail-length: 6.39em;
  --top-offset: 63.8vh;
  --fall-duration: 11.928s;
  --fall-delay: 5.531s;
  color: snow;
}
.star:nth-child(45) {
  --star-tail-length: 7.07em;
  --top-offset: 83.64vh;
  --fall-duration: 6.612s;
  --fall-delay: 8.726s;
  color: crimson;
}
.star:nth-child(46) {
  --star-tail-length: 6.64em;
  --top-offset: 94.9vh;
  --fall-duration: 11.947s;
  --fall-delay: 1.236s;
  color: darkgreen;
}
.star:nth-child(47) {
  --star-tail-length: 7.06em;
  --top-offset: 68.61vh;
  --fall-duration: 6.232s;
  --fall-delay: 5.158s;
  /* color: purple; */
}
.star:nth-child(48) {
  --star-tail-length: 5.54em;
  --top-offset: 23.83vh;
  --fall-duration: 9.165s;
  --fall-delay: 0.837s;
  /* color: purple; */
}
.star:nth-child(49) {
  --star-tail-length: 6.9em;
  --top-offset: 85.31vh;
  --fall-duration: 11.833s;
  --fall-delay: 9.208s;
  color: darkgreen;
}
.star:nth-child(50) {
  --star-tail-length: 6.91em;
  --top-offset: 50.51vh;
  --fall-duration: 11.263s;
  --fall-delay: 8.087s;
  color: chocolate;
}
.star::before, .star::after {
  position: absolute;
  content: "";
  top: 0;
  left: calc(var(--star-width) / -2);
  width: var(--star-width);
  height: 100%;
  background: linear-gradient(45deg, transparent, currentColor, transparent);
  border-radius: inherit;
  animation: blink 2s linear infinite;
}
.star::before {
  transform: rotate(45deg);
}
.star::after {
  transform: rotate(-45deg);
}

@keyframes fall {
  to {
    transform: translate3d(-30em, 0, 0);
  }
}
@keyframes tail-fade {
  0%, 50% {
    width: var(--star-tail-length);
    opacity: 1;
  }
  70%, 80% {
    width: 0;
    opacity: 0.4;
  }
  100% {
    width: 0;
    opacity: 0;
  }
}
@keyframes blink {
  50% {
    opacity: 0.6;
  }
}
</style>