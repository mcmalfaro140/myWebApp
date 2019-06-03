<template>
    <div class="menuBody">
       
        <ul class="nav justify-content-end">
            <li class="nav-item">
                <router-link to="/" class="nav-link txt">Home</router-link> 
            </li>
            <li class="nav-item">
                <router-link to="/portfolio" class="nav-link txt">Portfolio</router-link> 
            </li>
            <li class="nav-item">
                <router-link to="/resume" class="nav-link txt">Resume</router-link> 
            </li>
            <li class="nav-item">
                <router-link to="/contact" class="nav-link txt">Contact</router-link> 
            </li>
        </ul>
         
        
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
.menuBody{
    text-decoration: none;
    margin-right: 8%;
    padding: 2%;
    font-size: 175%;
    
    
}
.txt{
    color: white;
    font-weight: bold;
}
@media only screen and (max-width: 767px) {
  .menuBody{
    text-decoration: none;
    margin-right: 8%;
    padding: 3%;
    font-size: 140%;
    
  }
  .txt{
    font-weight: 500;   
  }
}


</style>
