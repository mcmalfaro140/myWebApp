<template>
<div>
    <div class="content">
        <project class="col item" v-bind:infoData="infoData"/>
        
    </div>
    <a class="git btn-primary btn-lg btn-block " href="https://github.com/mcmalfaro140" target="_blank">My GitHub Account</a>
    
</div>
</template>
<script>
import project from '../components/project'

export default {
    data () {
        return{
            infoData: [
                {
                    name: 'WeatherApp',
                    url: require('../assets/weatherApp.png'),
                    description:'This single page web application displays the weather by letting the user input a location. It uses the APIXU API. It is integrated in a node module to make JSON request to the API and manipulates DOM elements to display the weather.',
                    link: 'http://misaelweather.netlify.com',
                    repo: 'https://github.com/mcmalfaro140/weatherApp',
                    tech: [
                        {tec : 'JavaScript'},
                        {tec : 'Node.js'},
                        {tec : 'Apixu API'},
                        {tec : 'HTML/CSS'}
                    ],
                    learned: [
                        {point : 'To manipulate DOM elements with JavaScript.'},
                        {point : 'To creade node modules and integrate technologies like browserify and watchify to import multiple JavaScript in one file.'},
                        {point : 'To interpretate JSON response from an API.'},
                        {point : 'To desing for movil devices first and then create different media queries for different devices.'}
                    ]
                    
                },
                {
                    name: 'Todo List',
                    url: require('../assets/todo.png'),
                    description:'Single web application created with the react cli to add or delete task from a database.',
                    link: 'http://misaeltodos.netlify.com',
                    repo: 'https://github.com/mcmalfaro140/myTodos',
                    tech: [
                        {tec : 'JSX'},
                        {tec : 'Node.js'},
                        {tec : 'React.js'},
                        {tec : 'Bootsrap'}
                    ],
                    learned: [
                        {point : 'To develop web applications with React and its environment.'},
                        {point : 'To interpretate JSON response to my state.'},
                        {point : 'To develop a Full stack application.'}
                    ]
                    
                },
                {
                    name: 'Todo List Server',
                    url: require('../assets/server.png'),
                    description:'Restful API desing to get or modify data from my database. It is used as the backend for my Todo List application.',
                    link: 'http://todosmisael.herokuapp.com',
                    repo: 'https://github.com/mcmalfaro140/todo_server',
                    tech: [
                        {tec : 'Express.js'},
                        {tec : 'Node.js'},
                        {tec : 'mySql'},
                        
                    ],
                    learned: [
                        {point : 'To develop the backend for my application.'},
                        {point : 'To connect to my database and modify it.'},
                        {point : 'To create routes with express.'}
                    ]
                    
                },
                {
                    name: 'My Website',
                    url: require('../assets/website.png'),
                    description:'My own website created to show potential employers my abilities as a junior web desing. It was implemented with the integration of VUE CLI and vue-route to allow multiple pages.',
                    link: 'http://misaelcorvera.netlify.com',
                    repo: 'https://github.com/mcmalfaro140/myWebApp',
                    tech:[
                        {tec: 'VUE.js'},
                        {tec: 'Bootstrap'},
                        {tec: 'CSS'}
                    ],
                    learned: [
                        {point: 'To integrate different dependencies from vue to give a better overall user experience.'},
                        {point: 'To embed pdf files to allow users to see my resume.'},
                        {point: 'To create different media queries.'},
                        {point: 'To design a website by combining colors and shapes, as well as pictures to get the user attention.'}
                    ]
                    
                }
            ]
        }
    },
    components:{
        project
    }
}
</script>


<style scoped>
.content{
    color: black;
    
}
.git{
    text-align: center;
    font-size: 175%;
    width: 50%;
    margin-left: 25%;
    text-decoration: none;
}
@media only screen and (max-width: 768px) {
    .git{
        font-size: 125%;
    }
    .content{
        margin-top: 20%;
    }
    
}
</style>

