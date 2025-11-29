<template>
    <h1>Dynamic Component</h1>
    <node />
    <php />
    <java />
    <button v-on:click="tab='node'">Load Node</button>
    <button v-on:click="tab='php'">Load PHP</button>
    <button v-on:click="tab='java'">Load Java</button>

    <component :is="tab" />
    </template>
    <script>
    import node from './node.vue';
    import php from './php.vue';
    import java from './java.vue';
    export default {
        name: "Home",
        components: {
            node,php,java
        },
        data() {
            return {
                tab:'java'
            }
        }
    }
</script>
<style>
h1 {
    color: orange;
}
</style>