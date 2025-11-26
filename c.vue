<template>
<h1>Pass Data to child component</h1>
<child name="Bharat Tiwari" :user="user" :getData="getData" />
</template>

<script>
import child from './child.vue'
export default {
    name: "Home",
    components: {
        child
    },
    data() {
        return {
            user: {
                name: "Alisha",
                email: 'alisha@gmail.com'
            }
        }
    },
    methods: {
        getData() {
            console.log("parent function called")
            alert("Hello")
        }
    }
}
</script>

<style>
h1 {
    color: orange;
}
</style>
