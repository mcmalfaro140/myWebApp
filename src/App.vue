<template>
<div class="wrapper">
  
  <div id="app" >
      <Menu />
      <div class="container effect">
        <vue-page-transition name="fade-in-down">
          <router-view/>
        </vue-page-transition>
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
  margin:0%;
  padding: 0%;
  
}
.effect{
  -webkit-animation: fadein 4s; /* Safari, Chrome and Opera > 12.1 */
  -moz-animation: fadein 4s; /* Firefox < 16 */
  -ms-animation: fadein 4s; /* Internet Explorer */
  -o-animation: fadein 4s; /* Opera < 12.1 */
  animation: fadein 4s;
}

@keyframes fadein {
    from { opacity: 0; }
    to   { opacity: 1; }
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
@media only screen and (min-width: 768px) {
   
    
}

</style>
