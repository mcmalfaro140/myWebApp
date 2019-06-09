<template>
<div class="wrapper">
  <div id="app" class="trans">
      <Menu />
      <div class="container">
        <router-view/>
      </div>
    
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
  background-image: url('./assets/back.jpg');
  background-position: center; 
  background-repeat: no-repeat; 
  background-size: cover; 
  height: 100vh;
  background-attachment: fixed;
   
}
.wrapper{
  width: 100%;
}
.container{
  margin-top: 9%;
  
}
.content{
    background-color: rgba(245, 245, 245, 0.562);
    border-radius: 25px;
    padding: 2%;
    margin:auto;
    margin-bottom: 3%;
    text-align: center;
    
}

</style>
