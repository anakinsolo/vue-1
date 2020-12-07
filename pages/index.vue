<template>
  <div class="container">
    <div>
      <Logo />
      <h1 class="title">
        vue-1
      </h1>
      <div class="links">
        <a
          href="https://nuxtjs.org/"
          target="_blank"
          rel="noopener noreferrer"
          class="button--green"
        >
          Documentation
        </a>
        <a
          href="https://github.com/nuxt/nuxt.js"
          target="_blank"
          rel="noopener noreferrer"
          class="button--grey"
        >
          GitHub
        </a>
      </div>
      <div> {{hello}} </div>
      <button class="button--green" v-on:click="helloMethod">Click me mon </button>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from 'vue'

export default Vue.extend({
  data () {
    return {
      hello: 'Hello Mon!!!'
    }
  },
  methods: {
    helloMethod () {
      this.hello = 'Hello Click'
    }
  }
})
</script>
