<template>
  <div id="app" class="trans">
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

/* html {
  
  background-image: url('./assets/back.jpg');
  background-position: center; 
  background-repeat: no-repeat; 
  background-size: cover; 
  height: 100vh;
  background-attachment: fixed;
  
 
}

body {
  background:rgba(0, 0, 0, 0.479); 
  height:max-content;
 
} */
body{
  background-image: url('./assets/back1.jpg');
  background-position: center; 
  background-repeat: no-repeat; 
  background-size: cover; 
  height: 100vh;
  background-attachment: fixed;
 
}
@media only screen and (max-width: 767px) {
  body{
    
    
  }
}
@media only screen and (max-width: 1920px) {
  body{
     height: 100vh;
    
  }
}


</style>
