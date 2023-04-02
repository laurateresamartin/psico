<template>
  <div>
  <div class="head">
        <section class="contact-head">
          <div class="contact">
              <div class="contact-telefono" style="display:flex;align-items: center;">
                 <img
                class="burguer"
                src="../../assets/telefono.png"
                alt=""
                height="15px"
                style="margin-top: -2px;"
                />
                <h2 style="font-weight: 600; margin-left: 10px;     margin-bottom: 6px;">
                  <a class="text-contact" style="color: white; text-decoration: none;" href="tel:+674409610"
                    >000000000</a
                  >
                </h2>
              </div>
              <div class="contact-correo" style="display:flex;align-items: center; margin-left: 30px">
                 <img
                  class="burguer"
                  src="../../assets/correo.png"
                  alt=""
                  height="15px"
                  style="margin-top: -2px;"
                  />
                  <h2 style="font-weight: 600; margin-left: 10px; margin-bottom: 6px;">
                    <a class="text-contact" style="color: white; text-decoration: none" href=""
                      >dwjwejdn@kikewjdew.com</a
                    >
                  </h2>
              </div>

          </div>
          <div class="icon-redes">
               <nav class="social-links">
                <a
                  href=""
                  class="social-link"
                  target="_blank"
                >
                  <img
                    class="burguer"
                    src="../../assets/instagram.png"
                    alt=""
                    height="30px"
                    style="margin-top: -4px;"
                  />
                </a>
              </nav>
          </div>
        </section>
        <section class="head-menu" style="height: 100px;">
           <nav>
              <ul class="sidebar-panel-nav">
                <li class="link-only"  :class="{
                      active:
                        '/inicio' === $route.path,
                    }">
                     <a :href="'/inicio'"

                     >Inicio</a>
                </li>
                <li class="link-only"  :class="{
                      active:
                        '/sobreMi' === $route.path,
                    }">
                    <a :href="'/sobreMi'"

                    >Sobre mi</a>
                </li>
 <img
                    class="burguer"
                    src="../../assets/gato.png"
                    alt=""
                    height="90px"
                    style="    padding: 0px 0px 0px 50px;;margin-top: -25px;"
                  />
                <li class="link-only" :class="{
                      active:
                        '/terapiasYservicios' === $route.path,
                    }">
                  <a :href="'/terapiasYservicios'"

                  >Terapias y Servicios</a>
                </li>
                <li class="link-only" :class="{
                      active:
                        '/preguntasFrecuentes' === $route.path,
                    }">
                  <a :href="'/preguntasFrecuentes'"

                  >Preguntas Frecuentes</a>
                </li>
              </ul>
            </nav>
        </section>
    </div>
  </div>
</template>

<script lang="ts">
import Vue from "vue";
import { mapGetters, mapMutations } from "vuex";

export default Vue.extend({
  name: "NavBar",
  components: {
  },
  computed: {
    ...mapGetters({ drawer: "drawer/getDrawerState" }),
  },
  props: {

  },
  methods: {


    ...mapMutations({ toggle: "drawer/toggle", hide: "drawer/hide" }),
  },
});
</script>

<style lang="postcss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@100&display=swap');
.contact-head{
    display: flex;
    justify-content: space-between;
    position: relative;
    width: 100%;
    height: 30px;
    transition: background 0.3s, border 0.3s, border-radius 0.3s, box-shadow 0.3s;
    padding: 3px 12px 3px 12px;
    background-color: #bde1cd;
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
  padding-top: 30px;
  list-style-type: none;
  justify-content: center;
}

.sidebar-panel-nav > li {
      margin-left: 30px;
  color: #8b878b;
  text-decoration: none;
  font-size: 1.1rem;
  height: 50px;
  display: block;
  padding: 10px 15px;

  &:hover {
    color: #8b878b;
  }


}
ul{
    display: flex;
}

.active {
   border-bottom: 3px #b2d5c2 solid;
   font-weight: 600;
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
