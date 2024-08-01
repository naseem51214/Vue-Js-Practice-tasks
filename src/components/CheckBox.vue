<template>
    <h1>
        Checkbox & Radio buttons
    </h1>
    <h3>Technologies</h3>
    <label for="java">Java</label>
    <input type="checkbox" value="java" id="java" v-model="technology">
    <label for="php">PHP</label>
    <input type="checkbox" value="php" id="php" v-model="technology">
    <label for="node">Node</label>
    <input type="checkbox" value="node" id="node" v-model="technology">
    <br> <br>
    <h3>Who I am </h3>
    <label for="student">Student</label>
    <input type="radio" value="student" id="student" name="who" v-model="who">
    <label for="developer">Developer</label>
    <input type="radio" value="developer" id="developer" name="who" v-model="who">
    <h3>Selected Technologies: {{ technology }}</h3>
    <h3>I am a : {{ who }}</h3>

</template>

<script>
export default {
    name: 'CheckBox',
    data() {
        return {
            technology:[],
            who:null,
        }
    },

}
</script>