<template>
<h1>HTML Binding</h1>
<h1>{{ text }}</h1>
<div v-html="tag"></div>
<div v-html="tag2"></div>
</template>

    
<script>
export default {
    name: "Home",
    data () {
        return {
            text: "Bharat Tiwari",
            tag:"<h1>Bhanu</h1>",
            tag2:"<h1>Bhanu@gmail.com</h1>"
        }
    }
}
</script>

<style scoped>
h1{
    color:orange;
}
</style>