<template>
  <div class="home">
    <img src="../assets/me.jpg" alt="myPic" class="myPic">
    <div class="hi">Welcome!</div>
    <div class="text">my name is <span class="name">Misael Corvera.</span></div>
    <div class="text">I am an enthusiastic junior web developer</div>
    <div class="text">ready to help you achieve your goals</div>
    <div class="text">in a fast and efficient manner.</div>
    <a class="btn btn-primary btn-lg btn-block " href="../myResume.pdf" download="MisaelCorveraResume.pdf">Download my Resume</a>
    <br>
    <footer class="foot">MacBook Pro is a registered trademak of Apple, Inc.®</footer>
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
  margin-top: 5%;
  margin-left: 0%;
  border-radius: 5%;
  
  
}
.hi{
  color: white;
  margin-top: -30%;
  margin-left: 22%;
  font-size: 600%;
  text-shadow:
	  -1px -1px 0 #000,
		1px -1px 0 #000,
		-4px 4px 0 #000,
		1px 1px 0 #000;
    
}
.text{
  color: white;
  margin-left: 22%;
  font-size: 120%;
  border-left: 3px solid white;
  padding-left: 8px;
  
  
}
.name{
  color: white;
  font-size: 300%;
  text-shadow:
	  -1px -1px 0 #000,
		1px -1px 0 #000,
		-3px 3px 0 #000,
		1px 1px 0 #000;
}
.btn{
  margin-top: 4%;
  margin-left: 10%;
  width: 45%;
    
}
.foot{
  color: white;
  margin-top: 12%;
  margin-left: 45%;
  font-size: 60%;
}
@media only screen and (max-width: 768px) {
  .myPic{
    width: 45%;
    margin-left: 30%;
    margin-top: 5%;
    border-radius: 50%;
    border:  2px solid black;
    margin-bottom: 30%;
  }
  .hi{
    margin-left: 15%;
    font-size: 500%;

  }
  .name{
    font-size: 200%;
    
  }
  
  .btn{
    margin-top: 5%;
    width: 60%;
    margin-left: 15%;
      
  }
}

@media only screen and (max-width: 1024px) {
  .hi{
    margin-top: -35%;
  }
}


</style>

