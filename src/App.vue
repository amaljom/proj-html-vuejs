<template>
  <div id="app">
    <Header />
    <Main />
    <Footer />
  </div>
</template>

<script>
import Header from './components/header/Header'
import Main from './components/main/Main'
import Footer from './components/Footer'

export default {
  name: 'App',
  components: {
    Header,
    Main,
    Footer
  }
}
</script>

<style lang="scss">
@import "~bootstrap/scss/bootstrap.scss";
*{
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}
body{
  background-color: rgb(255, 255, 255);
  font-family: 'Fredoka One', cursive;
  font-family: 'Montserrat', sans-serif;
  font-family: 'Mukta', sans-serif;
  font-family: 'Nunito', sans-serif;
  font-family: 'Open Sans', sans-serif;
  font-family: 'PT Sans', sans-serif;
}
</style>
