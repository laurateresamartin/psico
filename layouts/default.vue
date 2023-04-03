<template>
  <div class="layout">
    <transition name="horizontal-slide">
      <navbar></navbar>
    </transition>
    <Nuxt id="content"> </Nuxt>
  </div>
</template>

<script lang="ts">
import navbar from "./NavBar/NavBar.vue";
import Vue from "vue";

export default Vue.extend({
  name: "Default",
  components: {
    navbar,
  },

  data() {
    return {
    };
  },
});
</script>

<style lang="postcss">
html,
body {
  min-width: 20rem;
  line-height: 1.3;
  scroll-behavior: smooth;
}

.layout {
  position: relative;
}

body {
  position: relative;
}

*,
*:before,
*:after {
  box-sizing: border-box;
  margin: 0;
}

*:focus {
  transition: none !important;
  outline: 2px solid var(--color-pink-light);
  outline-offset: 2px;
}

a[href^="tel:"] {
  white-space: nowrap;
}

.hl-link {
  cursor: pointer;
  text-decoration: underline;
  color: var(--color-pink-base);

  &:hover {
    text-decoration: none;
    color: var(--color-pink-dark);
  }
}

@media (--sm) {
  #content {
    margin-bottom: 11rem;
    height: 1000px;
  }
}
</style>
