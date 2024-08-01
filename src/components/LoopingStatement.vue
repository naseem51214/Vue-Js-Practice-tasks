<template lang="">
    <h1>
       Loop statement in Vue js 
    </h1>
    <ul>
        <li v-for="items in technology" :key="items">{{items}}</li>
    </ul>   
    <br>
    <br>

    <ul>
        <li v-for="user in users " :key="user.email">Name is: {{user.name}} and Email is: {{user.email}}</li>
    </ul> 

</template>

<script>
export default {
    name: "LoopingStatement",
    data() {
        return {
            technology:['HTML' , 'CSS' , 'Javascript' , 'Bootstrap' , 'TailwindCSS' , 'Reac'],
            users:[
                {name:'Anees',email:'anees@gmail.com'},
                {name:'Salam',email:'salam@gmail.com'},
                {name:'Jawad',email:'jawad@gmail.com'}
            ]
        }
    },
}
</script>