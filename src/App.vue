<template>
  <div id="app">
    <router-view/>
  </div>
</template>

<script>
import { mapState } from 'vuex'
export default {
  name: 'App',
  components: {
  },
  computed: mapState(['locale']),
  watch: {
    locale() {
      this.$router.replace({ params: { lang: this.locale } }).catch(() => {})
    }
  },
  created() {
    this.$store.dispatch('changeLocale', this.$store.state.locale)
  }
}
</script>

<style lang="scss">
@import url('https://use.typekit.net/uzx2elw.css');
@import './../node_modules/bulma/css/bulma.css';
@import './assets/scss/_colors.scss';

#app {
  font-family: 'Muli', sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #1d1d1f;
  padding-top: 15px;
}
.header-intro {
  padding: 5rem 0 5rem;
  background-color: #fafafa;
  margin-bottom: 5rem;
}
a {
  text-decoration: none;
}
</style>
