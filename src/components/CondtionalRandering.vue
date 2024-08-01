<template>
    <h1 v-if="show">
       If Statement 
    </h1>
    <h1 v-else>
       Else Statement 
    </h1>
    <button v-on:click="show=!show" type="button">Toggle</button>
</template>
<script>
export default {
    name:"CondtionalRandering",
    data() {
        return {
            show:false,

        }
    },
}
</script>

