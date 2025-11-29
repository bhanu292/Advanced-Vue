<template>
<h1>Slots in VUE js </h1>
<child><h1>Code step by step</h1></child>
</template>

    
<script>
import child from './child.vue';
export default {
    name: "Home",
    components: {
        child,
    }
}
</script>

<style>
h1 {
    color: orange;
}
</style>
