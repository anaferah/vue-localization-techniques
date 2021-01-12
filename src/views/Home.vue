<template>
  <main>
    <Header/>  
    <img alt="Vue logo" src="@/assets/logo.png" />
    <HelloWorld :msg="$t('hello')" />
    <div class="link">
      <router-link :to="{ name: 'about' }"> About </router-link>
    </div>
    <Footer/> 
  </main>
</template>

<script>
import HelloWorld from '@/components/HelloWorld.vue'
import Header from '@/components/Header.vue'
import Footer from '@/components/Footer.vue'


export default {
  name: 'home',
  components: {
    HelloWorld,
    Header,
    Footer
  }
}
</script>
<style lang="scss">

</style>
