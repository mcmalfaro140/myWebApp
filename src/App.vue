<template>
  <div id="app">
      <Menu />
      <div class="container">
        <router-view/>
      </div>
    
  </div>
</template>

<script>
import Menu from './components/menu'
export default {
  name : 'app',
  components : {
    Menu
  }
}
</script>


<style>

html {
  background-image: url('./assets/back.jpg');
  background-position: center; 
  background-repeat: no-repeat; 
  background-size: cover; 
  height: 100vh;
  background-attachment: fixed;
}

body {
  background:rgba(0, 0, 0, 0.342); /* applies a 50% transparent white background */
  height: 100vh;
  background-attachment: fixed;
  
}
@media only screen and (max-width: 767px) {
  body{
    height: 200vh;
    
  }
}
</style>
