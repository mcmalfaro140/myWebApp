<template>
    <div class="bar">
        <nav class="navbar fixed-top navbar-expand-lg navbar-dark">
            <span class="d-lg-none d-xl-none">Misael Corvera</span>
            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarNavAltMarkup" aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon "></span>
            </button>
            <div class="collapse navbar-collapse justify-content-end" id="navbarNavAltMarkup">
                <div id="navBar" class="navbar-nav  nav-text ">
                    <router-link  to="/" class="nav-item nav-text">Home</router-link> 
                    <router-link to="/portfolio" class="nav-item nav-text">Portfolio</router-link>
                    <router-link to="/resume" class="nav-item  nav-text">Resume</router-link>
                    <router-link to="/contact" class="nav-item nav-text">Contact</router-link> 
                </div>
            </div>
        </nav>
    </div>
</template>

<script>
export default {
    
    }
</script>

<style scoped>
.bar {
    font-size: 175%;
    color:white;
    font-weight: 450;
   
                 
}
.bar nav{
    background-color:rgba(0, 0, 0, 0.671);
    
    }
.nav-text{
   margin-right: 10%;
    color: rgb(255, 255, 255);
    padding: 0.5%
}
.nav-item:hover{
    text-decoration: none;
    color:rgb(218, 214, 30);
    font-size: 110%;
    padding: 0%;
}

</style>
