<template>
    <h1>
        Pass data to child component
    </h1>
    <ChildComponent name="Anees" :user="user" :getData="getData"/>
</template>

<script>
import ChildComponent from './ChildComponent.vue';
export default {
    name: 'ParentComponent',
    components:
    {
        ChildComponent
    },
    data() {
        return {
            user:{name:'Anees',email:'anees@test.com'}
        }
    },
    methods:{
        getData(){
            console.warn('parent data')
            alert("parent data")
        }
    }
}
</script>