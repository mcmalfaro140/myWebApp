<template>
  <div class="home">
    <div class="cont">
      <div class="container">
        <div class="row">
          <div class="col-sm-5 col-md-6 left">
            <div class="nameBlock"> 
              Misael Corvera
              <div class="title">Computer Engineer</div>
            </div>
            <div class="welcomeBlock"> 
              Welcome, Thanks for visiting!
            </div>
            <div class="para">

              <p>Thanks for checking out my site!</p>
              <p>aksjdhaksdn alsdkjlkasdj alksdjlaksjd laksjdlkasdj laksjdlkaj lasjdal.</p>
              <p>aksjdhaksdn alsdkjlkasdj alksdjlaksjd laksjdlkasdj laksjdlkaj lasjdal.</p>
              <p>aksjdhaksdn alsdkjlkasdj alksdjlaksjd laksjdlkasdj laksjdlkaj lasjdal.</p>
              <p>aksjdhaksdn alsdkjlkasdj alksdjlaksjd laksjdlkasdj laksjdlkaj lasjdal.</p>
              <p>aksjdhaksdn alsdkjlkasdj alksdjlaksjd laksjdlkasdj laksjdlkaj lasjdal.</p>
              <p>aksjdhaksdn alsdkjlkasdj alksdjlaksjd laksjdlkasdj laksjdlkaj lasjdal.</p>
              <p>aksjdhaksdn alsdkjlkasdj alksdjlaksjd laksjdlkasdj laksjdlkaj lasjdal.</p>
              <p>aksjdhaksdn alsdkjlkasdj alksdjlaksjd laksjdlkasdj laksjdlkaj lasjdal.</p>
              <p>aksjdhaksdn alsdkjlkasdj alksdjlaksjd laksjdlkasdj laksjdlkaj lasjdal.</p>
              



            </div>
            
          </div>
          <div class="col-sm-5 offset-sm-2 col-md-6 offset-md-0" >
            <div class="row">
              <img src="../assets/myPic.jpg" alt="myPic"  class="rounded mx-auto d-block myPhoto" />
            </div>
            <div class="row info">
              <table class="table table-borderless">
                <thead>
                  <tr class="infoHead">
                    Information
                  </tr>
                </thead>
                <tbody>
                  <tr>
                    <td>Name:</td>
                    <td><h5>Misael Corvera Alfaro</h5></td>
                  </tr>
                  <tr>
                    <td>Locarion:</td>
                    <td><h5>Los Angeles, CA.</h5></td>
                  </tr>
                  <tr>
                    <td>Phone:</td>
                    <td><h5>818-239-6835</h5></td>
                  </tr>
                  <tr>
                    <td>Email: </td>
                    <td><h5>mcmalfaro140@gmail.com</h5></td>
                  </tr>
                </tbody>
              </table>

              <button type="button" class="btn btn-primary btn-lg btn-block">Download My Resume</button>
              
            </div>
            
            
          </div>
        </div>
      </div>
    </div>
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
body{
  background-image: linear-gradient(black, white);
  min-height: 100vh;
  
}
.cont{
  background-color: white;
  margin-block-start: -6%;
  margin-left: 4%;
  margin-right: 4%;
  height: 750px;
  margin-bottom: 3%;
}
.myPhoto{
  width: 50%;
  height: 300px;
  transform: rotate(-90deg);
  margin-block-start: 10%;
  
  
}
.nameBlock{
  margin-top: 6%;
  background-color: rgb(21, 84, 179);
  color: white;
  font-family:'Georgia',serif;
  letter-spacing: 5px;
  padding: 2%;
  margin-top: 12%;
  font-size: 300%;
  
}
.welcomeBlock{
  background-color: rgb(211, 211, 224);
  text-align: center;
  font-size: 200%;
  font-style: italic;
  padding: 3%;
}
.info{
  margin-left: 13%;
  
}
.infoHead{
  color: rgb(24, 9, 224);
  font-size: 200%;
  font-weight: bold;
}

.title{
  background-color:white;
  text-align: right;
  color: black;
  font-size: 30%;
}
.para{
  padding: 3%;
}

</style>

