<template>
  <div id="app">
    <div id="appBarWrapper">
      <AppBarWrapper></AppBarWrapper>
    </div>
    <div id="searchSectionContent">
      <SearchSectionContent></SearchSectionContent>
    </div>

    <img alt="Vue logo" src="./assets/logo.png">
    
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue'
//import MiComponente from './components/MiComponente.vue'
import AppBarWrapper from './components/AppBarWrapper.vue'
import SearchSectionContent from './components/SearchSectionContent.vue'

export default {
  name: 'App',
  components: {
    AppBarWrapper,
    SearchSectionContent
  },
  data() {
    return {
      todos: [
        {
          id: 0,
          title: 'dsda',
          complete: false
        }       
      ]
    }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 0px;
}

#appBarWrapper {
  height: 25%;
  width: 100%;
  position: absolute;
}

#searchSectionContent {
  height: 75%;
  width: 100%;
  position: absolute;
  top: 25%;
}
</style>
