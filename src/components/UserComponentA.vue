<template>
    <div>
        
        <h2>
            {{ meta.name }}
        </h2>
        <h2>
            {{ meta.email }}
        </h2>
        <button v-on:click="abc(meta.name)">Alert Name</button>
    </div>
</template>
<script>
export default {
    name:'UserComponentA',
    props:{
        meta:Object,
        abc:Function,
    }
}
</script>

<style scoped>
div{
    background-color: lightseagreen;
    padding: 5px;
    margin: 5px;
    border: 1px solid;
    border-radius: 5px;
    width: auto;
    max-width: 200px;
}
h2{
    margin-left: 5px;
}

</style>