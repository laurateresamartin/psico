<template>
  <div class="wrapper">
    <link rel="shortcut icon" href="#" />
     <menuApp>
      <menucontainer />
    </menuApp>
     <main>
      <router-view />
    </main>
  </div>
</template>

<script>
import navbar from "../layouts/NavBar/NavBar.vue";
import menuApp from "../components/Menu/Menu.vue";
import menucontainer from "../components/Menu/MenuContainer.vue";
import home from "./home/Home.vue";
export default {
  layout: "default",
  name: "Home",
  components: {
    menuApp,
    navbar,
    menucontainer,
    home,
  },
  head: {
    title: "Home",
  },
};
</script>
