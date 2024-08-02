<template>
    <h1>
        Wacher property in vue js example
    </h1>
    
        <button v-on:click="counter=counter-1">-</button>
           <span>{{ counter }}</span> 
        <button v-on:click="counter=counter+1">+</button>
        <br>
        <br>
    

</template>

<script>
export default {
    name: 'WacherProperty',
    data() {
        return {
            counter: 0
        }
    },
    watch:{
        counter(cur,prev){
            if(cur>5 && cur>prev){
            
                alert('Stop increasing')
            }
        }
    }
}
</script>
<style scoped>
span{
    margin-left: 70px;
}
</style>