<template>
<h1>Ref in vue.js 3</h1>
<input type="text" ref="input" />
<button v-on:click="getData">Click me</button>
</template>

    
<script>
export default {
    name: "Home",
    methods: {
        getData () { 
            this.$refs.input.focus();
            let val= this.$refs.input.value;
            console.log(val);
             this.$refs.input.style.color="red"
        }
    }
}
</script>

<style>
h1 {
    color:orange;
}
</style>