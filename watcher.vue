<template>
    <h1>Watchers</h1>
    <h2>{{ count }}</h2>
    <button v-on:click="count=count+1"> + </button>
    <button v-on:click="count=count-1"> - </button>
    </template>

    <script>
export default {
    name: "Home",
    data () {
        return {
            count:0
        }
    },
    watch: {
        count (val,prev) {
            if(val>5 && val>prev){
             this.count=0
            }
        }
    }
}
</script>
<style>
h1 {
    color:orange;
}
</style>