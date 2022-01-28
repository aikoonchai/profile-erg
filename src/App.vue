<template>
  <div id="app">
    <NavigationBar/>
    <PanelPics/>
    <AboutMe/>
    <Experiences/>
    <Contact/>
  </div>
</template>

<script>
import NavigationBar from './components/NavigationBar.vue'
import PanelPics from './components/PanelPics.vue'
import AboutMe from './components/AboutMe.vue'
import Experiences from './components/Experiences.vue'
import Contact from './components/Contact.vue'

export default {
  name: 'App',
  components: {
    NavigationBar,
    PanelPics,
    AboutMe,
    Experiences,
    Contact
  }
}
</script>

<style>
*{
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  margin: 0;
  padding: 0;
  border: 0;
}
</style>
