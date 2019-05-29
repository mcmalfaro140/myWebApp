<template>
    <div>
        <div class="blackBar"/>
        <div class="menu" >
            <router-link to="/" class="header">Home</router-link> 
            <router-link to="/portfolio" class="header">Portfolio</router-link> 
            <img class="logo" alt="My logo" src="../assets/Logo.png">
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
    text-align: center;
}

.logo {
    width: 15%;

}
.header{
    text-decoration: none;
    color: black;
    vertical-align:450%;
    font-size: 195%;
    font-weight: bolder;
    padding: 4%

}
</style>
