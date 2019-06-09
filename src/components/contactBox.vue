<template>
<div>
    <div class="box" v-for="info in infoData" v-bind:key="info.name">
        <h2>{{info.name}}</h2>
        <br>
        <img class="logo" v-bind:src="info.url" alte="hello">
        <br>
        <h5>{{info.text}}</h5>
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
.box{
    background-color: white;
    border-radius: 25px;
    width: 70%;
    height: 30%;
    padding: 2%;
    text-align: center;
    margin: auto;
    margin-bottom: 2%;
    
}
.box h5{
    margin: 3%
}
.logo{
    width: 10%
}
@media only screen and (max-width: 768px) {
    .box{
    margin-bottom: 4%;
    width: 100%;
    }
    .logo{
        width: 15%
    }
}

</style>
