<template>
<h1>Send Data Child to Parent</h1>
<user :getUser="getuserName" />
<h2>{{ childUser }}</h2>
</template>

    
<script>
import user from './user.vue'
export default {
    name: "Home",
    data () {
        return {
            childUser:""
        }
    },
    components: {
        user
    },
        methods: {
            getuserName(name) {
                this.childUser=name
            }
        }
}
</script>

<style>
h1 {
    color: orange;
}
</style>
