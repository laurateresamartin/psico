<template>
  <div class="sidebar">
    <transition name="slide">
      <div v-if="drawer" class="sidebar-panel">
        <slot> </slot>
      </div>
    </transition>
  </div>
</template>

<script lang="ts">
import { mapGetters, mapMutations } from "vuex";

export default {
  name: "Menu",
  methods: {
    ...mapMutations({ toggle: "drawer/toggle" }),
  },
  computed: {
    ...mapGetters({ drawer: "drawer/getDrawerState" }),
  },
};
</script>

<style lang="postcss" scoped>

</style>
