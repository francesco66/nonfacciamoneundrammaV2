<template>
  <div class="mailtoui">
    <a class="link grow br3 ba bw1 pa2 bg-animate hover-bg-light-purple bg-black-60 white dib" :href="mailtoHref">
      <svg class="bg-white" xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24"><path d="M20 4H4c-1.1 0-1.99.9-1.99 2L2 18c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 4l-8 5-8-5V6l8 5 8-5v2z"/></svg>
    </a>
  </div> 
</template>

<script>
export default {

  props: {
    article: Object
  },

  computed: {
    mailtoHref: function() {
      //const email = "mailto:francescoarmandoporta@gmail.com?subject=" + encodeURI(this.article.path) + "&body=" + encodeURI(this.$replaceText2(this.article.text));
      const email = "mailto:francescoarmandoporta@gmail.com?subject=" + encodeURI(this.article.path) + "&body=" + encodeURI(this.article.text);
      return email;
    }
  }

}
</script>

<style scoped>
</style>