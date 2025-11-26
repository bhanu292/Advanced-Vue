<template>
<h1 v-if="show">IF Condition</h1>
<h1 v-else> ELSE Condition</h1>
<button v-on:click="show=!show">Toggle</button>
</template>

    
<script>
export default {
    name: "Home",
    data() {
        return {
            show: true
        }
    }
}
</script>

<style>
h1 {
    color: orange;
}
</style>
