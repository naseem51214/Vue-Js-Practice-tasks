<template>
    <h1>
        Ref Keyword Example in Vue js
    </h1>
    <input type="text" ref="input">
   
    <button v-on:click="getData">Click</button>
    <br>
    <br>
</template>

<script>
export default {
    name:'RefKeyWord',
    methods:{
        getData(){
        this.$refs.input.focus();
        let val = this.$refs.input.value;
        console.warn(val);
        this.$refs.input.style.color = 'red';
    }
    }
    
}
</script>