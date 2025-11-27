<template>
<h1>User Component</h1>
<button v-on:click="getUser(userName)">Send User Name</button>
</template>

    
<script>
export default {
    name: "user",
    data() {
        return {
            userName: 'Bhasker'
        }
    },
    props: {
        getUser: Function
    }

}
</script>
