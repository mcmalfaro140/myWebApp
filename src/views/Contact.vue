<template>
    <div class="content row">
        <contBox class="col item" v-bind:infoData="infoData"/>
        
    </div>
</template>

<script>
import contBox from '../components/contactBox'

export default {
    data () {
        return{
            infoData: [
                {
                    name: 'By Phone',
                    url: require('../assets/telephone.png'),
                    text:'1-818-239-6835',
                    link: 'tel:1-818-239-6835'
                    
                },
                {
                    name: 'By Email',
                    url: require('../assets/mail.png'),
                    text:'mcmalfaro140@gmail.com',
                    link: 'mailto:mcmalfaro140@gmail.com'
                },
                {
                    name: 'By Social Media',
                    url: require('../assets/insta.png'),
                    text:'@misaelcorvera',
                    link: 'http://www.instagram.com/misaelcorvera'
                }
            ]
        }
    },
    components:{
        contBox
    }
    
}
</script>

<style scoped>

@media only screen and (max-width: 768px) {
    .item{
        width: 700%
    }
    .content{
        margin-top: 20%;
    }
}

</style>


