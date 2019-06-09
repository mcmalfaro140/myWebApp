<template>
<div>
    <div class="" v-for="info in infoData" v-bind:key="info.name">
        <div class="boxes">
        <h2>{{info.name}}</h2>
        <br>
        <img class="logo" v-bind:src="info.url" alte="hello">
        <br>
        <h5><a v-bind:href="info.link">{{info.text}}</a></h5>
        </div>
    </div>
    
</div>

</template>

<script>

export default {
    name:'contBox',
    props: ["infoData"]

    
}
</script>

<style scoped>
.boxes{
    background-color: white;
    border-radius: 25px;
    width: 70%;
    height: 30%;
    padding: 2%;
    text-align: center;
    margin:auto;
    margin-bottom: 2%;
    
}
.box h5{
    margin: 3%
}
.logo{
    width: 10%
}

.boxes:hover{
    transition: background-color 0.5s ease;
    background-color: rgba(62, 160, 252, 0.945);
  
    
}

@media only screen and (max-width: 768px) {
    .boxes{
    margin-bottom: 4%;
    width: 100%;
    }
    .logo{
        width: 15%
    }
}

</style>
