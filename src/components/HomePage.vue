<template>
    <h1>
        Get input value
    </h1>
    <div>
        <input type="text" placeholder="Enter email" v-model="email" />
        <br>
        <br>
        <input type="password" placeholder="Enter password" v-model="password" />
        <br><br>
        <button @click="getData">Get Metadata</button>

    </div>

</template>

<script>
export default {
    name: "HoemPage",
    data() {
        return {
            email:null,
            password:null,
        }
    },
    methods:{
        getData(){
            console.log('values:' ,this.email, this.password)
        }
    }
}
</script>

<style>
h1 {
    color: orange;
}
button{
    margin-left: 85px;
}
</style>