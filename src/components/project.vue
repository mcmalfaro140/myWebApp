<template>
<div>
    
    <div class="box" v-for="info in infoData" v-bind:key="info.name">
        <div class="divLine"></div>
        <div class="row">
            <div class="imageBox col-md-5">
                <div class="hovereffect hBox">
                    <img class="img-responsive screen" v-bind:src="info.url" alt="">
                    <div class="overlay">
                    <h2>{{info.name}}</h2>
                    <a class="info" v-bind:href="info.link" target="_blank">Link here</a>
                    </div>
                </div>
                <div class="picDes">Hover the picture for link.</div>
            </div>
            <div class="description col-md-6">
                <h1>{{info.name}}</h1>
                <h4>Description:</h4>
                <p>{{info.description}}</p>
                <h4>Technology used:</h4>
                <ul>
                    <li v-for="item in info.tech">
                        {{item.tec}}
                    </li>
                </ul>
                <h4>What I learned:</h4>
                <ul>
                    <li v-for="item in info.learned">
                        {{item.point}}
                    </li>
                </ul>
                <h6>Link:</h6>
                <a v-bind:href="info.link" target="_blank">{{info.link}}</a>
                <div class="repo">
                    <h6>GitHub Repository:</h6>
                    <a v-bind:href="info.repo" target="_blank">{{info.repo}}</a>
                </div>
            </div>
        </div>
        <div class="divLine"></div>
    </div>
</div>
</template>

<script>
export default {
    name: 'project',
    props: ["infoData"]
}
</script>


<style scoped>
.box{
    background-color: white;
    margin: 0%;
    margin-bottom: 2%;
    padding: 2%;
    border-radius: 5px;
    width: auto;
    
}
.screen{
    width: 100%;
   
    
}
.imageBox{
    width: 40%;
    max-height: 250px;
    margin: 2%;
    /* display: flexbox; */
}
.hBox{
     border: 1px solid black;
     border-radius: 5px;
}
.description{
    text-align: left;
}
.divLine{
    border: 1px solid black;
    margin: 3%
}
.hovereffect {
  width: 100%;
  height: 100%;
  /* float: left; */
  overflow: hidden;
  position: relative;
  text-align: center;
  cursor: default;
}

.hovereffect .overlay {
  width: 100%;
  height: 100%;
  position: absolute;
  overflow: hidden;
  top: 0;
  left: 0;
  -webkit-transition: all 0.4s ease-in-out;
  transition: all 0.4s ease-in-out;
}

.hovereffect:hover .overlay {
  background-color: rgba(170,170,170,0.4);
}

.hovereffect h2, .hovereffect img {
  -webkit-transition: all 0.4s ease-in-out;
  transition: all 0.4s ease-in-out;
}

.hovereffect img {
  display: block;
  position: relative;
  -webkit-transform: scale(1.1);
  -ms-transform: scale(1.1);
  transform: scale(1.1);
}

.hovereffect:hover img {
  -webkit-transform: scale(1);
  -ms-transform: scale(1);
  transform: scale(1);
}

.hovereffect h2 {
  text-transform: uppercase;
  color: #fff;
  text-align: center;
  position: relative;
  font-size: 17px;
  padding: 10px;
  background: rgba(0, 0, 0, 0.6);
  /* margin-top: 2%; */
}

.hovereffect a.info {
  display: inline-block;
  text-decoration: none;
  padding: 7px 14px;
  text-transform: uppercase;
  color: #fff;
  border: 1px solid #fff;
  /* margin: 0px 0 0 0; */
  margin-top: 25%;
  background-color: transparent;
  opacity: 0;
  filter: alpha(opacity=0);
  -webkit-transform: scale(1.5);
  -ms-transform: scale(1.5);
  transform: scale(1.5);
  -webkit-transition: all 0.4s ease-in-out;
  transition: all 0.4s ease-in-out;
  font-weight: bolder;
  font-size: 120%;
  height: 30%;
  width: 85%;
  position: absolute;
  top: -20%;
  left: 8%;
  padding: 70px;
}

.hovereffect:hover a.info {
  opacity: 1;
  filter: alpha(opacity=100);
  -webkit-transform: scale(1);
  -ms-transform: scale(1);
  transform: scale(1);
  background-color: rgba(0,0,0,0.4);
}
@media only screen and (max-width: 768px) {
    .picDes{
        visibility: hidden;
    }
    .imageBox{
        width: 100%;
        max-height: 250px;
        
    }
    .hBox{
     border: none;
    }
    .box{
        margin-bottom: 5%
    }
    .repo{
        display: none;
    }
    
}

</style>

