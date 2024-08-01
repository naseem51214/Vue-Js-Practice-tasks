<template>
    <h1>
        Teacher {{ name }}
    </h1>
</template>

<script>
export default {
    name:'TeacherComponent',
    props:{
        name:String
    }
}
</script>