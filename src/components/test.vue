<template>
<div>
<div v-html="myhtml"></div>
    <div v-if="showname">{{user.firstname}} </div>
    <div v-else="showname">No te conozco carnal</div>
    <hr>
    
    <ul>
        <li v-for="task in tasks">
    {{task.title}}
    </li>
    
    </ul>
    
    </div>
</template>

<script>
export default{
    data(){
        return{
            title:"Mi primer app con vue.js",
            user:{
                firstname:'sergio',
                lastname: 'aguilera'
            },
            myhtml:'<h3>Hola Vue</h3>',
            showname:false,
            tasks:[
                
                {title:'MTG'},
                {title:'DM'},
                {title:'DND'},
            ]
        }
    }
    
}
</script>

<style media="screen">

</style>