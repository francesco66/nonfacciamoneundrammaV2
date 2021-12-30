<template>
  <div @click="show = !show" >

    <input
      v-model="searchQuery"
      type="search"
      autocomplete="off"
      placeholder="Cerca"
      class="ba bw1 pa2 ml3 bg-animate hover-bg-light-purple bg-black-50 white dib"
    />
      <ul
        v-show="show"
        v-if="articles.length"
        class="modal-mask bg-black ba bw1 b--white br3 pt3 pb3"
      >
        <li class="blue" v-for="article of articles" :key="article.slug">
          <NuxtLink
            :to="{ name: nome, params: { slug: article.slug } }"
            class="white-80 dim no-underline underline-hover pr2"
          >
          {{ article.titolo + " di " + article.autore }}
          </NuxtLink>
        </li>
      </ul>

   </div>
</template>

<script>
export default {

  props: [ 'directory', 'nome' ],

  data() {
    return {
      searchQuery: '',
      articles: [],
      show: false
    }
  },

  watch: {
    async searchQuery(searchQuery) {
      if (!searchQuery) {
        this.articles = []
        return
      }

      this.articles = await this.$content(this.directory)
        .limit(10)
        .search(searchQuery)
        .fetch()

    }
  },

}
</script>

<style scoped>
.modal-mask {
  position: fixed;
  z-index: 9998;
  display: table;
  text-align: left;
  transition: opacity 0.3s ease;
}

</style>