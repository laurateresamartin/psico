<template>
  <div class="home" style="margin-top: -25px;">
    <div class="cover">

    </div>

  </div>
</template>

<script>
import Vue from "vue";
import navbar from "../../layouts/NavBar/NavBar.vue";

export default Vue.extend({
  layout: "default",
  components: {
    navbar
  },
  head: {
    title: "María psicóloga",
  },
});
</script>

<style lang="postcss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@100&display=swap');
.contact-head{
    display: flex;
    justify-content: space-between;
    margin-left: -8px;
    position: relative;
    width: 100%;
    height: 30px;
    transition: background 0.3s, border 0.3s, border-radius 0.3s, box-shadow 0.3s;
    padding: 3px 12px 3px 12px;
    background-color: #b2d5c2;
}
.head-menu {
    box-shadow: 0px 10px 10px 0px rgb(0 0 0 / 5%)

}
.icon-redes {
  margin-right: 30px;
}
.contact {
    display: flex;
    margin-left: 20px;
}
.text-contact{
  font-family: "Montserrat", Sans-serif;
    font-size: 14px;
    font-weight: 600;
}
#nav a.router-link-exact-active {
  color: #ffffff;
}
.sidebar-panel-nav {
    font-family: "Montserrat", Sans-serif;
    padding-top: 33px;
  list-style-type: none;
  justify-content: center;
}
.footer-container {
      text-align: center;
      display: flex;
      justify-content: space-around;
      .part-one {
        display: flex;
        align-items: center;
        margin-top: 10px;
      }
      .telephone {
        display: flex;
        margin-top: 40px;
        .phone {
          display: none;
        }
      }
    }
  .footer {
      height: 130px;
      background-color: #f6f6f6;
      position: fixed;
      right: 0;
      left: 0;
    }

.sidebar-panel-nav > li {
      margin-left: 30px;
  color: #8b878b;
  text-decoration: none;
  font-size: 1.1rem;
  display: block;
  padding-bottom: 1rem;

  &:hover {
    color: #8b878b;
  }
}
ul{
    display: flex;
}

.sidebar-panel-nav > li > a {
  color:  #141314;;
  text-decoration: none;
  font-size: 1.1rem;


  &:hover {
    color: #d494d4;
  }
}
</style>
