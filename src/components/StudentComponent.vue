<template>
    <h1>
        Student {{ name }}
    </h1>
</template>

<script>
export default {
    name:'StudentComponent',
    props:{
        name:String
    }

}
</script>