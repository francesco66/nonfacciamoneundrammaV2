<template>
  <div>

    <nav class="flex justify-between items-center w-100 bb bg-purple v-mid pa2 tc">
      <div class="flex fl ml4-l ml2">
        <PrevNext :prev="prev" nome="blogMDMA-slug" />
        <PrevNext :next="next" nome="blogMDMA-slug" />
      </div>
      <div class="flex tc pa2">
        <NuxtLink class="f2-l f3 link grow br3 ba bw1 pa2 bg-animate hover-bg-light-purple bg-black-60 white" :to="{ name: 'mdma' }">MDMA</NuxtLink>
      </div>
      <div class="flex fr pa2 mr4-l mr2">
        <buttonDownload class="mr2" :article="article" />
        <buttonEmailCorrezioni class="ml2" :article="article" />
      </div>
    </nav>

    <article class="pa3 pa5-ns">
      <h2 class="measure lh-copy">{{ article.autore }}</h2>
      <h1 class="f2 f1-l f-headline-l">{{ article.titolo }}</h1>
      <!-- <span class="measure lh-copy ma5" v-if="article.data">{{ article.data }}</span> -->

      <embed v-if="article.video"
        type="video/webm"
        :src="article.video"
        width="250"
        height="200">

      <p class="measure lh-copy">
        <nuxt-content :document="article" type="text/plain;charset=utf-8"/>
      </p>
    </article>

  </div>
</template>

<script>
export default {

  async asyncData({ $content, params } ) {

    const directory = "articlesMDMA";
    const article = await $content(directory, params.slug, { 'text': true }).fetch()

    const [prev, next] = await $content(directory)
      .only(['titolo', 'autore'])
      .sortBy('titolo', 'asc')
      .surround(params.slug)
      .fetch()

    return {
      article,
      prev,
      next,
    }
  },

}
</script>
