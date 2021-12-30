<template>
  <div class="flex justify-between">
    <NuxtLink
      v-if="prev"
      :to="{ name: nome, params: { slug: prev.slug } }"
      class="link grow br3 ba bw1 pa2 bg-animate hover-bg-light-purple bg-black-60 white"
    >
      <svg viewBox="0 0 24 24" width="24" height="24" fill="white" xmlns="http://www.w3.org/2000/svg">
        <path d="m19.2 2.43-2.422-2.43-11.978 12 11.978 12 2.422-2.43-9.547-9.57z"/>
      </svg>
    </NuxtLink>
    <span v-else>&nbsp;</span>
    <NuxtLink
      v-if="next"
      :to="{ name: nome, params: { slug: next.slug } }"
      class="link grow br3 ba bw1 pa2 bg-animate hover-bg-light-purple bg-black-60 white"
    >
      <svg viewBox="0 0 24 24"  width="24" height="24" fill="white" xmlns="http://www.w3.org/2000/svg">
        <path d="m4.8 21.57 2.422 2.43 11.978-12-11.978-12-2.422 2.43 9.547 9.57z"/>
      </svg>
    </NuxtLink>
    <span v-else>&nbsp;</span>
  </div>
</template>

<script>
export default {

  props: {
    nome: String,
    prev: {
      type: Object,
      default: () => null
    },
    next: {
      type: Object,
      default: () => null
    }
  },

}
</script>
