<template>
    <h1>
        HTML Binding Example
    </h1>

    <div v-html="tag"></div>
</template>

<script>
export default {
    name:'HtmlBinding',
    data() {
        return {
            tag:'<h1>Hello I am HTML Binding</h1>'
        }
    },
}
</script>