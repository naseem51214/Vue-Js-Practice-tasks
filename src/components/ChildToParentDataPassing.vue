<template>
    <h1>
        Child to Parent data Passing Example
    </h1>
    <button v-on:click="getUserDAta(uerData)">Get Data</button>
</template>
<script>
import { Function } from 'core-js';

export default {
    name: 'ChildToParentDataPassing',
    data() {
        return {
            uerData:'my Data'
        }
    },
    props:{
        getUserDAta:Function
    }
}
</script>