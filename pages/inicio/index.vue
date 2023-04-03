<template>
  <div>
      <div class="background">

      </div>
  </div>
</template>


<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
mounted(){
  console.log('dentro');

}
})
</script>

<style lang="postcss" scoped>
.background {
  background-image: url('../../assets/inicio.jpg');
  background-size: cover;
    width: 100%;
    padding-top: 110%;

    height: 650px !important;
    position: absolute;
    background-position: center;
    top: var(--header-height);
    right: 0;
    left: 0;
    z-index: 0;
    padding: 2rem 3rem 5rem;
}
</style>
