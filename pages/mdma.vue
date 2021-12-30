<template>
  <!-- pagina principale del blog MDMA Mai Dire Mi Arrendo -->
  <div id="bg-img" class="center repeat" >

    <nav class="db dt-l w-100 border-box bb b--dark-blue bg-black-50 pa3 ph5-l center">
      <div class="db dtc-l v-mid w-100 w-10-l tc tl-l mb2 mb0-l">
        <NuxtLink class="dib link grow pa3 br3 ba bw1 bg-animate hover-bg-light-purple bg-black f4-l f6 white" to="/">Home</NuxtLink>
      </div>
      <div class="db dtc-l v-mid w-100 w-80-l tc mb2 mb0-l">
        <h1 class="dib baskerville f3 f1-l fw5 white">MAI DIRE MI ARRENDO</h1>
      </div>
      <div class="db dtc-l v-mid w-100 w-10-l tc tr-l">
        <AppSearchInput class="dib" directory="articlesMDMA" nome="blogMDMA-slug" />
      </div>
    </nav>

    <div class="flex flex-wrap justify-around pa3">
      <a v-for="article of articles" :key="article.slug">
        <NuxtLink :to="{ name: 'blogMDMA-slug', params: { slug: article.slug } }" class="link underline-hover purple">
          <div class="w-100 pa3 ma1 br3 bg-black grow">
            <embed v-if="article.video"
              type="video/webm"
              :src="article.video"
              width="250"
              height="200">
            <img v-else style="background-image" :src="article.img" class="db bg-center br3 cover" />
            <h3 class="f5 f5-ns mt2 mb0 white-90 tc">{{ article.titolo }}</h3>
            <h3 class="f6 f5 fw4 mt2 white-60 tc">{{ article.autore }}</h3>
          </div>
        </NuxtLink>
      </a>
    </div>
  </div>
</template>

<script>
export default {

  async asyncData({ $content }) {
    const articles = await $content('articlesMDMA')
      .sortBy('titolo', 'asc')
      .fetch()

    return {
      articles
    }
  },

}
</script>

<style scoped>
#bg-img {
  background-image: url("~/static/bg-207659.jpg");
}
</style>
