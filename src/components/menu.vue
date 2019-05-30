<template>
    <div>
        <div class="blackBar"/>
        <div class="menu" >
            <img class="logo" alt="My logo" src="../assets/Logo.png">
            <router-link to="/" class="header test">Home</router-link> 
            <router-link to="/portfolio" class="header">Portfolio</router-link> 
            <router-link to="/resume" class="header">Resume</router-link> 
            <router-link to="/contact" class="header">Contact Me</router-link> 
        </div>
        
        
        
    </div>
</template>

<script>
export default {
    
}
</script>

<style scoped>
.blackBar{
    border-top: 15px solid black;
    margin-left: 4%;
    margin-right: 4%

}
.menu{
    text-align: left;
    margin-left: 4%;
    margin-right: 4%;
    background-color: black;

}

.logo {
    width: 12%;
}
.header{
    text-decoration: none;
    color: white;
    vertical-align:80%;
    font-size: 150%;
    font-weight: bold;
    padding: 4%;
    

}
.test{
    background-color: white;
    border-radius: 20px;
    color: rgb(0, 0, 0);
    padding-top: 1%;
    font-size: 200%;
    
}
</style>
