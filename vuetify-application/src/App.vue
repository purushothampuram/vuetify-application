<template>
  <div id="app">
    <v-app>
      <v-content app wrap>
        <EmailSubscribe></EmailSubscribe>
        </v-content>
    </v-app>
  </div>
</template>

<script>
import EmailSubscribe from './components/EmailSubscribe'
export default {
  name: 'App',
  components: {EmailSubscribe}
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
