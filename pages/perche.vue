<template>
  <div class="w-100 vh-100 bg-blue">
    <nav class="db dt-l w-100 border-box pa3 ph5-l bg-black">
      <!-- <a class="db dtc-l v-mid w-100 w-25-l tc tr-l"> -->
      <div class="db dtc-l v-mid w-100 w-10-l tc tr-l">
        <NuxtLink class="link outline pa2 mb3 mb0-l dim white f6 f5-l fw6 dib" to="/" title="Home">Home</NuxtLink>
      </div>
      <div class="db dtc-l v-mid w-100 w-90-l tc tr-l">
        <NuxtLink class="link dim white f6 f5-l fw6 dib mr3 mr4-l" to="/chisiamo" title="Chi siamo">Chi siamo</NuxtLink>
        <NuxtLink class="link dim white f6 f5-l fw6 dib mr3 mr4-l" to="/dovesiamo" title="Dove siamo">Dove siamo</NuxtLink>
        <NuxtLink class="link dim white f6 f5-l fw6 dib" to="/contatti" title="Contatti">Contatti</NuxtLink>
      </div>
    </nav>

      <h1 class="w-100 white-80 f-headline-l lh-solid-l f1 lh-title tc">Perché?</h1>
      <div class="flex flex-wrap justify-around center items-center">
        <div class="w-40-l w-90 bb ba br3 bw2 b--dark-red tc bg-orange mb0-l mb4">
          <h1 class="white-80 f1-l lh-title-l f2 lh-copy tc">MDMA</h1>
          <p class="">Mai Dire Mi Arrendo è un gruppo di ...</p>
          <div class="pa4-l pa2">
            <a class="f4-l f5 link white-80 hover-dark-blue" href="mailto:mdma@nonfacciamoneundramma.org">mdma@nonfacciamoneundramma.org</a>
          </div>
        </div>
        <div class="w-40-l w-90 bb ba br3 bw2 tc bg-dark-green">
          <h1 class="white-80 f1-l lh-title-l f2 lh-copy tc">NDI</h1>
          <p class="">Nel Dominio dell'Incerto è un gruppo di ...</p>
          <div class="pa4-l pa2">
            <a class="f4-l f5 link white-80 hover-dark-blue" href="ndi@nonfacciamoneundramma.org">ndi@nonfacciamoneundramma.org</a>
          </div>
        </div>
      </div>

  </div>
</template>
