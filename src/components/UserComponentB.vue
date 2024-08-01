<template>
    <h1>
        Resue Component
    </h1>

    <ul>
        <li v-for="items in user" :key="items.email">

            <UserComponentA :meta="items"  :abc="getData"/>
            
        </li>
    </ul>
</template>

<script>
import UserComponentA from './UserComponentA.vue';

export default {
    name: 'UserComponentB',
    components: {
        UserComponentA,
    },
    data() {
        return {
            user: [
                { name: 'Anees', email: 'anees@test.com' },
                { name: 'Salam', email: 'salam@test.com' },
                { name: 'Jawad', email: 'Jawad@test.com' }
            ]
        }
    },
    methods:{
        getData(name)
        {
            alert(name)
        }
    }
}
</script>
<style scoped>
li {
    list-style: none;
    /* margin-left: 15px; */
}
ul{
    display: flex;
    /* flex-direction: column; */
    justify-content: first baseline;
}
</style>
