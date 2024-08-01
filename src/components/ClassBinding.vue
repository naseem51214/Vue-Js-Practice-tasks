

<template>
    <h1> Class Binding Example </h1>
    <h2 :class="applyStyle"> Component</h2>
    <button v-on:click="applyChange()">Apply Style</button>
  </template>
  
  <script>
  export default {
    name: 'ClassBinding',
    data() {
      return {
        colorFull: false
      }
    },
    methods:{
        applyChange(){
            this.colorFull=!(this.colorFull)
        }
    },
    computed: {
      applyStyle() {
        return {
          green: this.colorFull,
          err: true,
          other: true
        }
      }
    }
  }
  </script>
  
  <style>
  .green {
    background-color: green;
    width: auto;
    max-width: 250px;
    padding: 10px;
  }
  .err {
    color: red;
  }
  .other {
    font-size: 50px;
  }
  </style>