<template>
  <div>
    <v-card id="header" class="overflow-hidden">
      <v-app-bar
        data-app
        absolute
        dark
        height="100px"
        shrink-on-scroll
      >
        <v-avatar size="50" style="padding-top: 10px">
          <v-img src="../../public/static/personal.jpg" />
        </v-avatar>
        <v-spacer />
        <v-btn href="https://github.com/gnieto11" target="_blank" icon>
          <v-icon>mdi-github</v-icon>
        </v-btn>
        <v-btn href="https://www.linkedin.com/in/gonzalo-nieto-03508a199/" target="_blank" icon>
          <v-icon>mdi-linkedin</v-icon>
        </v-btn>
        <v-btn href="mailto:maurogonzalonieto2011@hotmail.com.ar" icon>
          <v-icon>mdi-email</v-icon>
        </v-btn>
        <!--        <v-menu offset-y>-->
        <!--          <template #activator="{ on, attrs }">-->
        <!--            <v-btn-->
        <!--              v-bind="attrs"-->
        <!--              icon-->
        <!--              v-on="on"-->
        <!--            >-->
        <!--              <v-app-bar-nav-icon />-->
        <!--            </v-btn>-->
        <!--          </template>-->
        <!--          <v-list>-->
        <!--            <v-list-item-->
        <!--              v-for="(item, index) in items"-->
        <!--              :key="index"-->
        <!--              @click="true"-->
        <!--            >-->
        <!--              <v-list-item-title>{{ item.title }}</v-list-item-title>-->
        <!--            </v-list-item>-->
        <!--          </v-list>-->
        <!--        </v-menu>-->
      </v-app-bar>
    </v-card>
    <div class="container">
      <presentation />
    </div>
  </div>
</template>
<script>
  import Presentation from '../components/Presentation'
  export default {
    name: 'Home',
    components: {
      Presentation
    },
    data () {
      return {
        items: [
          {id: 1, title: 'Sobre mi'},
          {id: 2, title: 'Tecnologías'},
          {id: 3, title: 'Proyectos'},
          {id: 4, title: 'Contactos'},
        ],
        inset: false,
      }
    }
  }
</script>

<style scoped>
  .container {
    transform: translate(0, 100px);
    //height: 100vh;
  }
  .divider {
    height: 0.01rem;
    background-color: black;
  }
</style>