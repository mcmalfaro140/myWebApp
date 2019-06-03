<template>
  <div class="home">
    <img src="../assets/myPic.png" alt="myPic" class="myPic">
    <div class="hi">Hello,</div>
    <div class="text">my name is <span class="name">Misael Corvera.</span></div>
    <div class="text">I am an enthusiastic junior web developer</div>
    <div class="text">ready to help you achieve your goals</div>
    <div class="text">in a fast and efficient manner.</div>
    <button type="button btn" class="btn btn-primary btn-lg btn-block ">Download my Resume</button>
    
  </div>
</template>

<script>
export default {
  name: 'home',
  components: {
    
  }
}
</script>

<style>
.myPic{
  width: 20%;
  margin-left: 10%
  
  
}
.hi{
  color: white;
  margin-left: 10%;
  font-size: 600%
  
  
}
.text{
  color: white;
  margin-left: 10%;
  font-size: 120%;
  border-left: 3px solid white;
  padding-left: 8px;
  
}
.name{
  color: white;
  font-size: 300%
}
.btn{
  margin-top: 2%;
  margin-left: 10%;
  width: 45%;
    
}
@media only screen and (max-width: 767px) {
  .myPic{
    width: 40%;
    margin-left: 30%;
    margin-top: 5%;
  }
}


</style>

