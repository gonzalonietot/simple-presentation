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
    }
  }
</script>

<style scoped>
  .container {
    transform: translate(0, 100px);
    //height: 100vh;
  }
</style>